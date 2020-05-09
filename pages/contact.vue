<template>
    <div class="containers">
        <nav>
            <input type="checkbox" id="nav" class="hidden">
            <label for="nav" class="nav-btn">
                    <i></i>
                    <i></i>
                    <i></i>
            </label>
            <div class="logo">
                    <nuxt-link to="/">HelloHasif</nuxt-link>
            </div>
            <div class="nav-wrapper">
                    <ul>
                        <li><nuxt-link to="/about">About</nuxt-link></li>
                        <li><nuxt-link to="/project">Projects</nuxt-link></li>
                        <li><nuxt-link to="/blog">Blogs</nuxt-link></li>
                        <li><nuxt-link to="/contact">Contact</nuxt-link></li>
                    </ul>
            </div>
        </nav>

        <div class="container my-12 mx-auto px-4 md:px-12">
            <!-- wrapper -->
          <section class="m-2 font-sans leading-normal flex wrap-sec">

          <!-- card container -->
          <div class="max-w-lg shadow-lg rounded overflow-hidden m-4 sm:flex ">
              <div class="h-48 sm:h-auto sm:w-48 md:w-64 flex-none bg-cover bg-center rounded rounded-t sm:rounded sm:rounded-l text-center overflow-hidden" style="background-image: url('/img/me-min1.jpg')">
              </div>
              
              <!-- card-content -->
              <div class="px-6 py-4">
              <h2 class="mb-2 font-black" style="font-family: 'Raleway', sans-serif; font-size: 18px;">Contact</h2>
              <div class="box" style="margin-top: 16px;">
                <div class="icon">
                  <ion-icon name="call"></ion-icon>
                  <a href="#" class="icon-text">+6013 631 5331</a>
                </div>

                <div class="whitespace1"></div>

                <div class="icon-mail">
                  <ion-icon name="mail"></ion-icon>
                  <a href="#" class="icon-text">hasifzulkifli95@gmail.com</a>
                </div>
              </div>

              <div class="whitespace1"></div>

              <div class="icon-locat">
                <ion-icon name="location"></ion-icon>
                <a href="#" class="icon-text">Cyberjaya, Selangor</a>
              </div>

              <div class="whitespace1"></div>

                <div class="icon-coffee">
                  <ion-icon name="cafe"></ion-icon>
                  <a href="#" class="icon-text">Coffee? Let's!</a>
                </div>

              <div class="whitespace1"></div>

                <div class="icon-coffee">
                  <ion-icon name="shield-checkmark"></ion-icon>
                  <a href="#" class="icon-text">Forever is really composed of nows </a>
                </div>



              <!-- <p class="mb-4 text-grey-dark text-sm">
                  Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cumque, recusandae!
              </p> -->
              
              </div>

          </div>
          
          </section>
        </div>
    </div>
</template>




<style>
* {
      box-sizing: border-box;
}

html {
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100vh;
}

body {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100vh;
  font-family: 'Poppins', sans-serif;
  font-weight: 300;
  background: url(/img/back2-min.jpg) no-repeat 50% 50%;
  background-position: center;
  background-size: cover;
}

nav {
  padding: 8px;
}

.logo {
  float: left;
  padding: 8px;
  margin-left: 16px;
  margin-top: 8px;
}

.logo a {
  color: #000;
  text-transform: uppercase;
  font-weight: 600;
  font-size: 18px;
  letter-spacing: 1px;
  text-decoration: none;

  transition: .4s;
}

.logo a:hover {
  background-color: black;
  color: white;
}

.whitespace1 {
    margin-top: 12px;
}

.wrap-sec {
  justify-content: center;
  margin-top: 14%;
}

.icon-text {
  font-size: 13px;
  margin-left: 8px;
  font-family: 'Raleway', sans-serif;

  font-weight: 500;
}


nav ul {
  float: right;
  margin-top: 1em;
}

nav ul li {
  display: inline-block;
  /* float: left; */
}

nav ul li:not(:first-child) {
  margin-left: 48px;
}

nav ul li:last-child {
  margin-right: 24px;
}

nav ul li a {
  display: inline-block;
  outline: none;
  color: #000;
  text-transform: uppercase;
  text-decoration: none;
  font-size: 14px;
  letter-spacing: 1.2px;
  font-weight: 600;

  transition: .4s;
}

nav ul li a:hover {
  background-color: black;
  color: white;
}

@media screen and (max-width: 864px) {
  .logo {
    padding: 0;
  }

  .content {
    position: absolute;
    top: 40%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .nav-wrapper {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    background: #fff;
    opacity: 0;
    transition: all 0.2s ease;
  }

  .nav-wrapper ul {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 100%;
  }

  .nav-wrapper ul li {
    display: block;
    float: none;
    width: 100%;
    text-align: right;
    margin-bottom: 10px;
  }

  .nav-wrapper ul li:nth-child(1) a {
    transition-delay: 0.2s;
  }

  .nav-wrapper ul li:nth-child(2) a {
    transition-delay: 0.3s;
  }

  .nav-wrapper ul li:nth-child(3) a {
    transition-delay: 0.4s;
  }

  .nav-wrapper ul li:nth-child(4) a {
    transition-delay: 0.5s;
  }

  .nav-wrapper ul li:not(:first-child) {
    margin-left: 0;
  }

  .nav-wrapper ul li a {
    padding: 10px 24px;
    opacity: 0;
    color: #000;
    font-size: 14px;
    font-weight: 600;
    letter-spacing: 1.2px;
    transform: translateX(-20px);
    transition: all 0.4s ease;
  }

  .nav-btn {
    position: fixed;
    right: 10px;
    top: 10px;
    display: block;
    width: 48px;
    height: 48px;
    cursor: pointer;
    z-index: 9999;
    border-radius: 50%;
  }

  .nav-btn i {
    display: block;
    width: 20px;
    height: 2px;
    background: #000;
    border-radius: 2px;
    margin-left: 14px;
  }

  .nav-btn i:nth-child(1) {
    margin-top: 16px;
  }

  .nav-btn i:nth-child(2) {
    margin-top: 4px;
    opacity: 1;
  }

  .nav-btn i:nth-child(3) {
    margin-top: 4px;
  }

  .about-content h2 {
    margin-top: 8%;
    margin-right: 2em;
    margin-left: 2em;
    font-family: 'Raleway', sans-serif;
    font-weight: 500;
    font-size: 14px;

    text-align: justify;
}
}

#nav:checked + .nav-btn {
  transform: rotate(45deg);
}

#nav:checked + .nav-btn i {
  background: #000;
  transition: transform 0.8s ease;
}

#nav:checked + .nav-btn i:nth-child(1) {
  transform: translateY(6px) rotate(180deg);
}

#nav:checked + .nav-btn i:nth-child(2) {
  opacity: 0;
}

#nav:checked + .nav-btn i:nth-child(3) {
  transform: translateY(-6px) rotate(90deg);
}

#nav:checked ~ .nav-wrapper {
  z-index: 9990;
  opacity: 1;
}

#nav:checked ~ .nav-wrapper ul li a {
  opacity: 1;
  transform: translateX(0);
}

.hidden {
  display: none;
}

.page-enter-active,
.page-leave-active {
  transition-property: opacity;
  transition-timing-function: ease-in-out;
  transition-duration: 600ms;
}
.page-enter,
.page-leave-to {
  opacity: 0;
}
</style>