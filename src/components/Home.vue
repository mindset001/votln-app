<template>
  <div class="head">

    <div class="left">
      <router-link to="/" tag="li">
        <img src="../assets/logo_name.png" alt="" style=" width: 93px; height: 27px; margin-left: 65px; margin-top:40px;" />
      </router-link>
      <img src="../assets/image1.png" alt="" class="phone"/>
    </div>
      
    <div class="hello">
      
      <div>
        <router-link to="/" tag= "li"><h1 class="hero">votln</h1></router-link>

      <h3>Hello, Welcome to votln.</h3>
      
      <div class="btn">
      <button class="join">Join a meeting</button>
      <button class="sign">
        <router-link to="/sign-in" tag= "li">Sign in</router-link>
      </button>
      
      </div>
      </div>
      
      <footer class="footer2">
        <img src="../assets/footerwave2.png" alt="" />
      </footer>
    <!-- <router-view></router-view> -->
  </div>
      <footer class="footer1">
        <img src="../assets/footerWave.png" alt="" />
      </footer>

  </div>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap");



.hello {
  position: relative;
  width: 100%;
  box-sizing: border-box;
  margin-top: 166px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  /* justify-content: center; */
}
.hero {
  color: #621a7b;
  font-family: ubuntu;
  font-size: 50px;
}

h3 {
  font-family: montserrat;
  font-weight: 550;
  font-size: 20px;
  line-height: 24px;
  letter-spacing: 0.02em;
  margin-top: 100px;
  color: #111111;
  font-style: normal;
}
.btn {
  display: flex;
  flex-direction: column;
  font-family: montserrat;
  margin-top: 30px;
}
button {
  font-family: montserrat;
  font-size: 20px;
  font-weight: 500;
  line-height: 24px;
  letter-spacing: 0.02em;
  border-radius: 10px;
  box-sizing: border-box;
  width: 318px;
  height: 50px;
}

.join {
  background-color: #621a7b;
  color: #ffffff;
}
.sign {
  margin-top: 20px;
  border: 1px solid #621a7b;
  box-sizing: border-box;
  border-radius: 10px;
  background-color: #fff;
}

.footer1 {
  
  display: none;
}
 .footer2 {
  position: absolute;
  bottom: -2px;
  /* left: 0; */
  right: 0;
}

  .head{
    display: flex;
    flex-direction: row;
  }
  .left{
    position: relative;
    z-index: 2;
    width: 100%;
    height: 100vh;
    background: linear-gradient(147.67deg, #72248D -7.44%, #54106B 111.12%);
    
  }
 
  .phone{
    position: absolute;
  bottom: 100px;
  /* left: 50px; */
  width: 100%;
  object-fit: cover;
    
  }

  @media only screen and (max-width: 525px) {

    .left{
      display: none;
    }
    .footer2{
      display:none;
    }

    .footer1{
      display: flex;
      /* displ */
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      overflow: hidden;
    }
    .hello{
      margin-top: 120px;
      
    }
    .head{
      height: 100vh;
      overflow: hidden;
    }
  }
  @media only screen and (max-width: 767px) {
  }

   @media only screen and (max-width: 991px) {
  }


</style>
