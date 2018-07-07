<template>
  <div class="row">
    <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12 topnave">
          <div class="header1">
            <img  src="../assets/mainlogo.png" height="60px" width="150px"/>
            <input type="text" name="search">
            <span class="glyphicon glyphicon-search topsearch"></span>
            <ul>
              <li><span class="glyphicon glyphicon-user"></span><a href="http://localhost:8082/#/Signup">SignUp</a></li>
              <li><span class="glyphicon glyphicon-log-in"></span><a href="http://localhost:8082/#/Login">LogIn</a></li>
            </ul>
          </div>
        </div>
      </div>
      <br>
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
          <div class="row">
            <div class="col-xs-4 col-sm-4 col-lg-4 col-md-4"></div>
            <div class="col-xs-4 col-sm-4 col-lg-4 col-md-4">
              <div class="log">
                <div class="row">
                  <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                    <img  src="../assets/logos.png" height="110px" width="100px">
                  </div>
                </div>
                <div class="row">
                  <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                    <label for="email">Enter Your Email</label>
                    <input type="email" name="email" placeholder="" id="email" value="" required v-model="email">
                  </div>
                </div>
                <br>
                <div class="row">
                  <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                    <label for="password">Enter Your Password</label>
                    <input type="password" name="password" placeholder="" id="password" value="" required v-model="password">
                  </div>
                </div>
                <br>
                <div class="row">
                  <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                    <div class="btn-medium" v-on:click="logins()">LOGIN</div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-xs-4 col-sm-4 col-lg-4 col-md-4"></div>
          </div>
        </div>
      </div>
      <br><br>
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12 foot3">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab obcaecati illo, maiores id et sapiente esse sed nobis explicabo, officiis suscipit dignissimos quibusdam. Impedit nulla repellat commodi placeat quos tempora!
        </div>
      </div>
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12 foot2">
          <div class="row">
            <div class="col-xs-3 col-sm-3 col-lg-3 col-md-3">
              <h3>lorem</h3>
              <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugit debitis suscipit neque autem eos, aut quae doloribus modi? Nulla sed fuga laboriosam dolorem provident dignissimos beatae ipsam et facere perspiciatis.</p>
            </div>
            <div class="col-xs-3 col-sm-3 col-lg-3 col-md-3">
              <h3>lorem</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem facere, iste reprehenderit porro, illum quia similique, dolorum assumenda recusandae at autem possimus repellendus nam optio quaerat animi earum delectus. Porro!</p>
            </div>
            <div class="col-xs-3 col-sm-3 col-lg-3 col-md-3">
              <h3>lorem</h3>
              <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Alias tempora esse eligendi, nisi fuga tenetur ea expedita deserunt rerum quis at, amet nostrum earum iure ipsum nam, delectus qui sapiente!</p>
            </div>
            <div class="col-xs-3 col-sm-3 col-lg-3 col-md-3">
              <h3>lorem</h3>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Perspiciatis doloribus quibusdam placeat minima et ea harum fugit error molestias quaerat cum, culpa, temporibus tenetur provident dicta totam ex quidem! Pariatur!</p>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12 foot1">
          <div class="row">
            <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
              <span class="glyphicon glyphicon-thumbs-up"></span>
            </div>
            <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
              <span class="glyphicon glyphicon-shopping-cart"></span>
            </div>
            <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
              <span class="glyphicon glyphicon-earphone"></span>
            </div>
            <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
              <span class="glyphicon glyphicon-search"></span>
            </div>
            <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
              <span class="glyphicon glyphicon-eye-open"></span>
            </div>
            <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
              <span class="glyphicon glyphicon-envelope"></span>
            </div>
          </div>
          <br>
          <div class="row">
            <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
              copyrightshifa@eshop.com
              <span class="social social-facebook"></span>
              <span class="social social-twitter"></span>
              <span class="social social-e-mail-envelope"></span>
              <span class="social social-youtube"></span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    logins: function () {
      alert('hai')
      let logEmail = this.email
      // alert(logEmail)
      let logPass = this.password
      let stEmail = this.$localStorage.get('email')
      // alert(stEmail)
      let stPass = this.$localStorage.get('pass')
      if (logEmail === stEmail && logPass === stPass) {
        alert('login sucessfully')
        this.$router.push({path: '/dashboard'})
        return true
      } else {
        alert('Invalid email or password')
        return false
      }
    }
  }
}
</script>
<style>
  .topnave {
    background-color: rgba(10, 20, 73, 0.925);
    text-decoration: none;
    position:fixed;
    z-index: 40;
    width:1800px;;
    height:70px;
    margin-top: -60px;
    padding-top: 20px;
    margin-left: 0px;
    background-attachment: fixed;
    background-size: cover;
  }
  .topsearch {
    color:#ff9900;
  }
  .header1 h3 {
    margin-left: 1%;
    margin-top: -0.5%;
    float: left;
  }
  .header1 h3:hover {
    color:thistle;
  }
  .header1 ul, li, a{
    color:gray;
    display: inline;
    margin: 0.5%;
    text-decoration: none;
    font-family: 'Raleway', sans-serif;
    font-size: bold 40px;
    padding-top: 10px;
  }
  .header1 ul, li, a:hover{
    color:#fff;
    text-decoration: none;
  }
  .nave {
    background-color: rgba(10, 20, 73, 0.925);
  }
  .topnave img {
    float: left;
  }
  .nave img {
    float: left;
  }
  .topnave img:hover {
    animation: shake 0.5s;
    animation-iteration-count: infinite;
  }

  @keyframes shake {
    0% { transform: translate(1px, 1px) rotate(0deg); }
    10% { transform: translate(-1px, -2px) rotate(-1deg); }
    20% { transform: translate(-3px, 0px) rotate(1deg); }
    30% { transform: translate(3px, 2px) rotate(0deg); }
    40% { transform: translate(1px, -1px) rotate(1deg); }
    50% { transform: translate(-1px, 2px) rotate(-1deg); }
    60% { transform: translate(-3px, 1px) rotate(0deg); }
    70% { transform: translate(3px, 1px) rotate(-1deg); }
    80% { transform: translate(-1px, -1px) rotate(1deg); }
    90% { transform: translate(1px, 2px) rotate(0deg); }
    100% { transform: translate(1px, -2px) rotate(-1deg); }
  }
  .log {
    width:300px;
    height:400px;
    border: #000;
    border:0px solid #000;
    background-image: url("");
    border-radius: .1em;
    padding-right: 5%;
    padding-top: 5%;
    padding-left: 10%;
    padding-bottom: 5%;
    color: #000;
    font: 1em sans-serif;
    box-shadow: 0 4px 20px 0 rgba(0,0,0,0.2);
  }
  .log input, text {
    font-size: 1em;
    display: block;
    width: 93%;
    padding:1em 1em 1em 0;
    background: none;
    background-image: none;
    border: none;
    border-bottom: 1px solid #8e8e8e;
    color: #000;
    border-radius: 0;
    -webkit-transition: border-color .25s ease, box-shadow .25s ease;
    -moz-transition: border-color .25s ease, box-shadow .25s ease;
    transition: border-color .25s ease, box-shadow .25s ease;
  }
  .log:hover {
    box-shadow: 0 8px 22px 0 rgba(0,0,0,0.2);
  }

  .log label {
    float: left;
  }

  .btn-medium {
    background-color:#ff9900;
    font-size: 14px;
    font-family: 'Roboto';
    text-align :center;
    color: white;
    width:90px;
    padding:10px;
    cursor: pointer;
    border-radius: 0.3em;
    text-decoration: none;
    box-shadow: 0 4px 2px 0 rgba(0.1,0.1,0.1,0.2);
  }

  .btn-medium:hover, .btn-medium:focus {
    background: #0c0c20;
    letter-spacing: 7px;
    box-shadow: 2px 2px 2px 2px rgba(1,0,0,0.1);
  }

  .btn-medium {
    display: block;
    width: 92%;
  }

  .foot3 {
    background-color: rgba(10, 20, 73, 0.925);
  }
  .foot2 {
    background-color: #111128;
  }
  .foot1 {
    background-color: #0C0C20;
  }
</style>
