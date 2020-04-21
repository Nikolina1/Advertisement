<template>
  <footer>
    <div class="main-content">
      <div class="left box">
        <h2>About us</h2>
        <div class="content">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti, optio! Eius, vero nesciunt? Facere commodi debitis sequi molestiae quis laboriosam saepe laborum accusantium vel nobis beatae, consectetur quo praesentium quae?</p>
          <div class="social">
            <a href="https://github.com/">
              <span>
                <i class="ion-social-github"></i>
              </span>
            </a>

            <a href="https://www.facebook.com/">
              <span>
                <i class="ion-social-facebook"></i>
              </span>
            </a>

            <a href="https://twitter.com/twitter">
              <span>
                <i class="ion-social-twitter"></i>
              </span>
            </a>

            <a href="https://www.instagram.com/">
              <span>
                <i class="ion-social-instagram"></i>
              </span>
            </a>
          </div>
        </div>
      </div>
      <div class="center box">
        <h2>Address</h2>
        <div class="content">
          <div class="place">
            <span class="ion">
              <i class="ion-ios-location"></i>
            </span>
            <span class="text">Čepić Polje, Kršan</span>
          </div>
          <div class="phone">
            <span class="ion">
              <i class="ion-ios-telephone"></i>
            </span>
            <span class="text">0915785031</span>
          </div>
          <div class="email">
            <span class="ion">
              <i class="ion-email"></i>
            </span>
            <span class="text">ljubicic.nikolina@gmail.com</span>
          </div>
        </div>
      </div>

      <div class="right box">
        <h2>Contact us</h2>
        <div class="content">
          <form action="#">
            <div class="email">
              <div class="text">Email *</div>
              <input type="email" required />
            </div>
            <div class="msg">
              <div class="text">Message *</div>
              <textarea cols="25" rows="2" required></textarea>
            </div>
            <div class="btn">
              <a href="mailto:ljubicic.nikolina@gmail.com">
                <button>Send</button>
              </a>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="bottom">
      <center>
        <span class="credit">
          Created By
          <a href="#">Nikolina</a> |
        </span>
        <span class="copyright">&copy; {{ new Date().getFullYear() }} All rights reserved.</span>
      </center>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter"
};
</script>
<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  color: #d9d9d9;
  font-family: "Manrope", sans-serif;
}

footer {
  bottom: 0px;
  width: 100%;
  background: #111;
}

.main-content {
  display: flex;
}

.main-content .box {
  flex-basis: 50%;
  padding: 10px 20px;
}

.box h2 {
  font-size: 1.125rem;
  font-weight: 600;
  text-transform: uppercase;
}

.box .content {
  margin: 20px 0 0 0;
  position: relative;
}

.box .content:before {
  position: absolute;
  content: "";
  top: -10px;
  height: 2px;
  width: 100%;
  background: #1a1a1a;
}

.box .content:after {
  position: absolute;
  content: "";
  height: 2px;
  width: 15%;
  background: #073b5e;
  top: -10px;
}

.left .content p {
  text-align: justify;
}

.left .content .social {
  margin: 20px 0 0 0;
}

.left .content .social a {
  padding: 0 2px;
}

.left .content .social a span i {
  height: 40px;
  width: 40px;
  background: #1a1a1a;
  line-height: 40px;
  text-align: center;
  font-size: 30px;
  border-radius: 5px;
  transition: 0.3s;
}
.left .content .social a span i:hover {
  background: #073b5e;
}

.center .content .ion {
  font-size: 1.4375rem;
  background: #1a1a1a;
  height: 45px;
  width: 45px;
  line-height: 45px;
  text-align: center;
  border-radius: 50%;
  transition: 0.3s;
  cursor: pointer;
}

.center .content .ion:hover {
  background: #073b5e;
}

.center .content .text {
  font-size: 1.0625rem;
  font-weight: 500;
  padding-left: 10px;
}

.center .content .phone {
  margin: 10px 0;
}

.right form .text {
  font-size: 1.0625rem;
  margin-bottom: 2px;
  color: #656565;
}

.right form .msg {
  margin-top: 10px;
}

.right form input,
.right form textarea {
  width: 100%;
  font-size: 1.0625rem;
  background: #151515;
  padding-left: 10px;
  border: 1px solid #222222;
}

.right form input:focus,
.right form textarea:focus {
  outline-color: #073b5e;
}

.right form input {
  height: 35px;
}

.right form .btn {
  margin-top: 10px;
}

.right form .btn button {
  height: 40px;
  width: 100%;
  border: none;
  outline: none;
  background: #073b5e;
  font-size: 1.0625rem;
  font-weight: 500;
  cursor: pointer;
  transition: 0.3s;
}

.right form .btn button:hover {
  background: #000;
}

.bottom center {
  padding: 5px;
  font-size: 0.9375rem;
  background: #151515;
}

.bottom center span {
  color: #656565;
}

.bottom center a {
  color: #073b5e;
  text-decoration: none;
}

.bottom center a:hover {
  text-decoration: underline;
}

@media screen and (max-width: 900px) {
  footer {
    position: static;
    bottom: 0px;
  }

  .main-content {
    flex-wrap: wrap;
    flex-direction: column;
  }

  .main-content .box {
    margin: 5px 0;
  }
}
</style>