<template>
  <div id="app">
    <div class="header-nav" id="nav">
      <div class="container">
        <div class="row align-items-end">
          <div class="header-logo col-md-3"><img src="./assets/images/logo.png" alt="LeoSpa"></div>
          <div class="header-nav__list col-md-9">
            <router-link to="/">Home</router-link>
            <router-link to="/about">About</router-link>
            <router-link to="/feature">Feature</router-link>
            <router-link to="/service">Service</router-link>
            <router-link to="/contact">Contact</router-link>
          </div>
        </div>
      </div>
    </div>

    <router-view/>

    <footer class="footer">
      <div class="container">
        <div class="row">
          <div class="col-12 text-center">
            <a href="/" class="logo footer__logo">
              <img src="./assets/images/logo.png" alt="logo">
            </a>

            <div class="footer-socials">
              <a class="footer-socials__link" href="#">
                <icon-facebook class="footer-socials__icon" />
              </a>
              <a class="footer-socials__link" href="#">
                <icon-twitter class="footer-socials__icon" />
              </a>
              <a class="footer-socials__link" href="#">
                <icon-vimeo class="footer-socials__icon" />
              </a>
              <a class="footer-socials__link" href="#">
                <icon-instagram class="footer-socials__icon" />
              </a>
            </div>
            <p class="copyright">&copy; COPYRIGHT 2019 <a href="https://themeies.com">themeies.com.</a> ALL RIGHTS RESERVED.</p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import IconFacebook from './components/IconFacebook.vue';
import IconInstagram from './components/IconInstagram.vue';
import IconTwitter from './components/IconTwitter.vue';
import IconVimeo from './components/IconVimeo.vue';
 
export default {
  name: 'App',
  components: {
    IconFacebook,
    IconInstagram,
    IconTwitter,
    IconVimeo,
  }
}
</script>

<style lang="scss">

#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;

  color: #6c6c6f;
  background-color: #fff;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
  font-size: 15px;
  line-height: 1.8;
}


.header-nav {
  &__list {
    text-transform: uppercase;
    a {
      color: inherit;
      margin-right: 40px;
      font-weight: 500;
      transition: all 0.3s ease;
      &:last-child {
        margin-right: 0;
      }
      &:hover {
        text-decoration: none;
        color: #ff817e;
      }

      &.router-link-exact-active {
        color: #ff817e;
      }
    }
  }
}
// #nav {}

.footer {
  background-color: #fff9f8;
  padding: 50px 0 50px;
  &__logo {
    display: block;
    margin-bottom: 30px;
  }
}
.footer-socials {
  margin-bottom: 30px;
  &__link {
    padding: 0 10px;
    font-size: 14px;
    border-right: 1px solid #b1b4bb;
    color: #3a414e;
  }
  &__icon {
    width: 14px;
    height: 14px;
    fill: #3a414e;
    color: #3a414e;
  }
  & a:hover {
    svg {
      fill: #ff817e;
      color: #ff817e;
    }
  }
}
</style>
