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

    
  </div>
</template>