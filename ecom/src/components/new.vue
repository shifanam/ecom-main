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
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
          <div class="row">
            <div class="col-xs-8 col-sm-8 col-lg-8 col-md-8"></div>
            <div class="col-xs-4 col-sm-4 col-lg-4 col-md-4 sign">
              <div class="row">
                <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                  <img  src="../assets/ss.png" height="80px" width="100px"/>
                </div>
              </div>
              <div class="row">
                <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                  <label for="email">Enter Email</label>
                  <input type="email" name="email" id="email" placeholder="example@gmail.com" v-model="email" required>
                </div>
              </div>
              <br>
              <div class="row">
                <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                  <label for="password">Enter Password</label>
                  <input type="password" name="password" id="password" placeholder="password" value="" v-model="password" required>
                </div>
              </div>
              <br>
              <div class="row">
                <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                  <div class="row">
                    <div class="col-xs-2 col-sm-2 col-lg-2 col-md-2">
                      <label class="check">
                        <input type="checkbox" id="checkbox"  v-on:click="myFunction()" checked="checked" name=check1 v-model="checkbox">
                        <span class="checkmark"></span>
                      </label>
                    </div>
                    <div class="col-xs-10 col-sm-10 col-lg-10 col-md-10">
                      <div class="show">
                        show password
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <br><br>
              <div class="row">
                <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                  <div class="btn-medium" v-on:click="form_validation()">SIGNUP</div>
                </div>
              </div>
              <br>
              <div class="row">
                <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
                  <div class="lo">
                    <i>click here to</i>
                      <a v-bind:href="url">Login</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-xs-4 col-sm-4 col-lg-4 col-md-4"></div>
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
  </div>
</template>
<script>
export default {
  data () {
    return {
      password: '',
      email: '',
      checkbox: '',
      url: 'http://localhost:8080/#/login'
    }
  },
  methods: {
    myFunction: function () {
      var x = document.getElementById('password')
      if (x.type === 'password') {
        x.type = 'text'
      } else {
        x.type = 'password'
      }
    },
    form_validation: function () {
      var email = this.email
      var password = this.password
      this.emailVal(email)
      this.passVal(password)
      this.testValidation(email, password)
      this.store(email, password)
    },
    emailVal: function (email) {
      var mailformat = /[A-Z0-9._%+-]+@[A-Z0-9.-]+.[A-Z]{2,4}/igm
      if (email.match(mailformat)) {
        return true
      } else {
        alert('Enter valid email!..')
        return false
      }
    },
    passVal: function (password) {
      let passformat = /^(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,16}$/
      if (password.match(passformat)) {
        return true
      } else {
        alert('Password should contain :atleast 1 alphabet,digit,special character and total 8-16 characters!..')
        return false
      }
    },
    store: function (email, password) {
      this.$localStorage.set('email', email)
      this.$localStorage.set('pass', password)
    },
    testValidation: function (email, password) {
      if (this.emailVal(email) === true && this.passVal(password) === true) {
        this.$router.push({path: '/login'})
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
body {
  background-image: url("");
  background-repeat: no-repeat;
  background-color: #fff;
  margin-top: -1%;
  margin-left: -1%;
  width:100%;
  margin-bottom: 0;
  text-decoration: none;
  background-attachment: fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  background-size: cover;
}

.nave-bar {
  background-color:none;
  display: block;
  height: 30px;
  width: 100%;
  text-decoration: none;
}

ul, li {
  list-style: none;
  display: block;
  overflow: hidden;
  margin: 0;
  padding-left: 12px;
  padding-top: 18px;
  float: left;
  top: 0;
  color: #fff;
  cursor: pointer;
}

a {
  text-decoration: none;
}

.s {
  width:1em;
  height:2em;

}
.sign {
  width: 30%;
  height:100%;
  border:0px solid #000;
  background-image: url("");
  background-color: #fff;
  padding-left: 5%;
  padding-top: 5%;
  padding-bottom: 5%;
  float: right;
  font: 1em sans-serif;
  border-radius: 1em;
  margin-right: 5%;
  box-shadow: 0 4px 20px 0 rgba(0,0,0,0.2);
  margin-top: -15%;
}
.sign:hover {
  box-shadow: 0 8px 22px 0 rgba(0,0,0,0.2);
}

input, text {
  font-size: 1em;
  display: block;
  width: 80%;
  padding:1em 1em 1em 0;
  background: none;
  background-image: none;
  border: none;
  border-bottom: 1px solid #8e8e8e;
  color: #000;
  text-align:left;
  border-radius: 0;
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
  width: 80%;
}

.check {
  display: block;
  position: relative;
  padding-left: 25px;
  padding-bottom: 12px;
  border:0px solid #000;
  cursor: pointer;
  font-size: 15px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.check input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
}

.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 20px;
  width: 20px;
  border: solid #ff9900;
  background-color: #eee;
}

.check:hover input ~ .checkmark {
  background-color: #aaa;
}

.check input:checked ~ .checkmark {
  background-color: #fff;
}

.checkmark:after {
  border: solid #122636;
  content: "";
  position: absolute;
  display: none;
}

.check input:checked ~ .checkmark:after {
  display: block;
}

.check .checkmark:after {
  left:6px;
  top: 3px;
  width: 4px;
  height: 8px;
  border:solid #ff9900;
  border-width: 0 3px 3px 0;
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
}

.show {
  margin-top: -1px;
  margin-left: -30px;
  float: left;
}

img {
  float: center;
  margin-left: -21%;
}

label {
  float: left;
}

.lo {
  color:#aaa;
  margin-top: -0.5px;
  margin-left: -30px;
  font-size: 0.8em;
}

.lo  a {
  color:rgb(221, 10, 10);
  font-size: 0.9em;
  text-decoration: none;
}

.design {
  font-size: 10%;
  font-family: 'Orbitron', sans-serif;
  color: #fff;
  margin-top: 13%;
  margin-left: 30px;
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
