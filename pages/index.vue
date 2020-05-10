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
                      <li><nuxt-link to="/">Home</nuxt-link></li>
                      <li><nuxt-link to="/about">About</nuxt-link></li>
                      <li><nuxt-link to="/project">Projects</nuxt-link></li>
                      <li><nuxt-link to="/blog">Blogs</nuxt-link></li>
                      <li><nuxt-link to="/contact">Contact</nuxt-link></li>
                </ul>
          </div>
    </nav>

    <div class="content">
          <span class="line1"><h1>Life has no limitations, except . .</h1></span>
          <span class="line22"><h1>the ones that you make it</h1></span>
    </div>
  </div>
</template>

<script>
export default {
 
}
</script>

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

.content {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.content .line1 {
  font-weight: 400;
  font-size: 28px;

  transition: .4s;
}

.content .line2 {
  font-weight: 300;
  font-size: 20px;

  transition: .4s;
  font-style: italic;
}

.content .line22 {
  font-weight: 300;
  font-size: 20px;

  transition: .4s;
  font-style: italic;
}

.content .line1:hover {
  /* background-color: white; */
  color: #000;
}

.content .line2:not(:hover) {
  color: #f4f5f7;
  
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

  .nav-wrapper ul li:nth-child(5) a {
    transition-delay: 0.6s;
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
