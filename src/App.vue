<template>
  <main>
    <div class="main-container">

        <div class="image-container"> 
          <div class="overlay">
            <img src="/images/icon-view.svg" alt="">
          </div>
        </div>
         <div class="text-container">
            <h4>Equilibrium #3429</h4>
            <p class="main-text">Our Equilibrium collection promotes balance and calm</p>
            <div class="price-date-container">
              <p class="price-container">
                <img src="/images/icon-ethereum.svg" alt="">
                0.014ETH
              </p>
              <p class="date-container">
                <img src="/images/icon-clock.svg" alt="">
                3 days left
            </p>
          </div>
         </div>
         <hr>

         <div class="avatar-container">
          <div class="avatar-image"></div>
          <p class="avatar-text">Creation of <span>Jules Wyvern</span></p>
         </div>
    </div>
  </main>
</template>

<style scoped>
  main{
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: hsl(217, 54%, 11%);
    box-shadow: 8px 8px 4px hsl(215, 51%, 70%);
  }

  .main-container{
    width: 350px;
    height: 550px;
    background-color: hsl(216, 50%, 16%);
    border-radius: 12px;
    padding: 20px;
    /* box-shadow: ; */
  }

  .image-container{
    width: 100%;
    height: 50%; 
    background-color: hsl(178, 100%, 50%);
    background-image: url("/images/image-equilibrium.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    border-radius: 9px;   
    position: relative;
  }

  h4{
    margin-top: 15px;
    margin-bottom: 10px;
    font-weight: 600;
    font-size: 18px;
    color: hsl(0, 0%, 100%);
  }

  p{
    font-size: 18px;
  }

  .main-text{
    font-weight: 400;
  }

  .price-date-container{
    display: flex;
    justify-content: space-between;
    margin-top: 15px;
  }

  .price-container{
    color: hsl(178, 100%, 50%);
    font-weight: 600;
  }

  .date-container{
    font-weight: 600;
  }

  hr{
    margin-top: 20px;
      height: 1px;
    background-color: hsl(215, 32%, 27%);
  }
 
  .avatar-container{
    display: flex;
    margin-top: 20px;
  }

  .avatar-image{
    width: 40px;
    height: 40px;
    background-image: url("/images/image-avatar.png");
    background-repeat: no-repeat;
    background-size: cover;
    border: 1px solid hsl(0, 0%, 100%);
    border-radius: 50%;
  }

  .avatar-text{
    margin-left: 20px;
    margin-top: 5px;
  }

  .avatar-text span{
    color:  hsl(0, 0%, 100%);
    margin-left: 5px;
  }

  h4:hover, span:hover{
    color: hsl(178, 100%, 50%);
    cursor: pointer;
  }

  .overlay {
    position: absolute;
    border-radius: 10px;
    width: 100%;
    height: 100%;
    background-color: hsl(178, 100%, 50%);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: all 0.3s ease-in;
  }

  .overlay:hover {
    opacity: 1;
    cursor: pointer;
  }
</style>