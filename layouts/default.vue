<template>
  <div class="wrapper">
    <header class="header">
      <div class="top-part">
        <b-container fluid>
          <b-row>
            <b-col sm="6">
              <a href="#">
                <i class="fab fa-facebook-square" />
              </a>
              <a href="#"><i class="fab fa-twitter-square"/></a>
              <a href="#"><i class="fab fa-youtube-square"/></a>
              <a href="#"><i class="fab fa-instagram-square"/></a>
            </b-col>
            <b-col sm="6" class="text-right">
              <a href="mailto:info@bijoytech.com"
                ><i class="fas fa-envelope"></i> info@bijoytech.com</a
              >
              &nbsp; &nbsp;
              <a href="tel:+8801688138948"
                ><i class="fas fa-phone-alt"></i> +88 01688 138948</a
              >
            </b-col>
          </b-row>
        </b-container>
      </div>
      <b-container fluid>
        <b-navbar toggleable="lg">
          <b-navbar-brand
            ><nuxt-link to="/">Bijoy Tech</nuxt-link></b-navbar-brand
          >
          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
          <b-collapse id="nav-collapse" is-nav>
            <!-- Right aligned nav items -->
            <b-navbar-nav class="ml-auto">
              <nuxt-link to="/about" class="nav-link">About us</nuxt-link>
              <nuxt-link to="/courses" class="nav-link">Courses</nuxt-link>
              <nuxt-link to="/services" class="nav-link">Services</nuxt-link>
              <nuxt-link to="/contact" class="nav-link">Contact us</nuxt-link>
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
      </b-container>
    </header>
    <nuxt />
    <footer class="footer">
      <b-container fluid>
        <b-row>
          <b-col md="4">
            <h1>Bijoy Tech</h1>
            Making a positive first impression is essential to developing a
            strong customer relationship. Ekko is powerful enough to assist any
            small businesses.
          </b-col>
          <b-col cols="4">
            <ul>
              <li><nuxt-link to="/about">About Us</nuxt-link></li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
            </ul>
          </b-col>
          <b-col md="4">
            <ul>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
              <li>
                <nuxt-link to="/about">About Us</nuxt-link>
              </li>
            </ul>
          </b-col>
        </b-row>
      </b-container>
    </footer>
  </div>
</template>

<style></style>
