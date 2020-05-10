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

    <div class="container my-12 mx-auto px-4 md:px-12">
        <div class="flex flex-wrap -mx-1 lg:-mx-4">
                  
                <div class="p-4 md:w-1/2">
                    <img src="/img/ms1.jpg" alt="" />
                </div>

                <div class="p-4 md:w-1/2">
                    <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa repellat laborum mollitia sequi magni! Amet facere sed beatae iste nulla accusamus? Vel esse, dolorem magni nisi quidem commodi odio, at eligendi reiciendis, harum fugiat obcaecati sapiente in quisquam modi sequi.</h2>
                </div>

        </div>
    </div>

    
  </div>
</template>