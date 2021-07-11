<template>
  <div class="head">

    <div class="left">
      <router-link to="/" tag="li">
        <img src="../assets/logo_name.png" alt="" style=" width: 93px; height: 27px; margin-left: 65px; margin-top:40px;" />
      </router-link>
      <img src="../assets/signup.png" alt="" class="phone"/>
    </div>
      
    <div class="hello">
        <router-link to="/">
        <img src="../assets/Vector.png" alt="" class="arrow" />
      </router-link>
      <div>
        <h1 class="hero">Sign Up</h1>

      <h3>create account and join your co-workers</h3>

      <form action="/action_page.php"> 
    <label for="phoneNumber">Phone Number</label> <br>
    <input type="text" id="phoneNumber" name="phoneNumber" placeholder="+234 816 007 1243"> <br>

    <label for="password">Password</label> <br>
    <input type="alphanumeric" id="password" name="password" placeholder="********">


    <div class="btn">
      <button class="join" type="submit">Sign Up</button>
      <button class="sign" >
        <router-link  tag= "li" to="/sign-in">Login</router-link>
      </button>
      
      </div>

          <div style="
              display: flex;
              flex-direction: row;
              margin-top: 20px;
              margin-bottom: 10px;
            ">
            <div class="line"></div>
            <!-- <img src="../assets/Line_1.png" alt="" style="width:100px; height: 1px;"/> -->
            <h4 class="with">or sign in with </h4>
            <div class="line"></div>
          </div>

      <div class="icons">
          <img src="../assets/sso.png" alt="" />
          <img src="../assets/google.png" alt="" />
          <img src="../assets/facebook.png" alt="" />
      </div>

  </form>
      
      
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

.with{
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 15px;
  padding-top:8px;
  margin-left: 10px;
  margin-right: 10px;
  color: #111111;
}

.icons{
  display: flex;
              justify-content: space-between;
              width: 150px;
              margin-left: 120px;
}

.arrow{
  display:none;
}
 
.hello {
  position: relative;
  width: 100%;
  box-sizing: border-box;
  margin-top: 61px;
  display: flex;
  flex-direction: column;
  align-items: left;
  text-align: left;
  padding-left: 200px;
  /* justify-content: center; */
}
.hero {
  color: #621a7b;
  font-family: ubuntu;
  font-size: 50px;
}

h3 {
  font-family: montserrat;
  font-weight: normal;
  font-size: 18px;
  line-height: 22px;
  letter-spacing: 0.02em;
  margin-top: 0px;
  color: #000000;
  font-style: normal;
}
.btn {
  display: flex;
  flex-direction: row;
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
  width: 188px;
  height: 40px;
}
form{
  margin-top: 40px;
}
label{
  font-family: monserrat;
  font-size: 18px;
  line-height: 22px;
  font-weight: normal;
}
input[type=text] {

  width: 397px;
  height: 50px;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 2px solid #621a7b;
  border-radius: 10px;
  box-sizing: border-box;
}
input[type=alphanumeric] {
   width: 397px;
  height: 50px;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 2px solid #c0c0c0;
  border-radius: 10px;
  box-sizing: border-box;
}

.join {
  background-color: #621a7b;
  color: #ffffff;
}
.sign {
  border: 1px solid #621a7b;
  box-sizing: border-box;
  border-radius: 10px;
  background-color: #fff;
  margin-left: 20px;
}

.footer1 {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
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
    bottom: 140px;
    left:120px;
    width: 60%;
  object-fit: cover;
    
  }
  .line{
       width: 146px;
                height: 1px;
                background-color: #dcc7e3;
                margin-top: 31px;
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
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      overflow: hidden;
    }
    .hello{
      margin-top: 20px;
      padding-left:45px;
      
    }
    .head{
      height: 100vh;
      overflow: hidden;
      align-items: center;
      justify-content: center;
    }
    input[type="text"]{
      width: 280px;
      height: 40px;
    }
    input[type="alphanumeric"]{
      width: 280px;
      height: 40px;
    }
    button{
      width: 130px;
      height: 45px;
    }
    .below{
      width: 280px;
    }
    h3{
      width: 300px;
      font-size: 16px;
    }
    .line{
      width: 94px;
    }
    .icons{
      margin-left: 60px;
      margin-bottom: 100px;
    }
    .arrow{
      display: block;
      width:16.6px;
      height:13.6px;
    }

     .arrow{
      display: block;
      width:16.6px;
      height:13.6px;
    }
  }


</style>
