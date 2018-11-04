<template>
    <v-layout align-center justify-center row fill-height>
        <v-flex xs5>
          <div class="logo">Atmosphonics</div>
        </v-flex>
        <v-flex>
          <ul class="main__nav">
            <li>How it works</li>
            <li>Solutions</li>
            <li>Features</li>
          </ul>
        </v-flex>
        <v-flex>
          <ul class="user__nav">
            <li class="user__nav--login">Login</li>
            <li class="user__nav--cta">Join Now</li>
          </ul>
        </v-flex>
        <div class="hidden-md-and-up text-xs-right burger__wrapper">
          <svg @click="showMobileMenu = !showMobileMenu" v-if="!showMobileMenu" aria-hidden="true" data-prefix="fas" data-icon="bars" class="fa-bars" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="currentColor" d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"></path></svg>
          <svg @click="showMobileMenu = !showMobileMenu" v-if="showMobileMenu" aria-hidden="true" data-prefix="fas" data-icon="times" class="fa-times" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 352 512"><path fill="currentColor" d="M242.72 256l100.07-100.07c12.28-12.28 12.28-32.19 0-44.48l-22.24-22.24c-12.28-12.28-32.19-12.28-44.48 0L176 189.28 75.93 89.21c-12.28-12.28-32.19-12.28-44.48 0L9.21 111.45c-12.28 12.28-12.28 32.19 0 44.48L109.28 256 9.21 356.07c-12.28 12.28-12.28 32.19 0 44.48l22.24 22.24c12.28 12.28 32.2 12.28 44.48 0L176 322.72l100.07 100.07c12.28 12.28 32.2 12.28 44.48 0l22.24-22.24c12.28-12.28 12.28-32.19 0-44.48L242.72 256z"></path></svg>
        </div>
        <div class="mobile__menu--wrapper" v-if="showMobileMenu">
          <ul class="mobile__menu">
            <li>How it works</li>
            <li>Solutions</li>
            <li>Features</li>
            <li>Login</li>
            <li>Join Now</li>
          </ul>
        </div>
      </v-layout> <!-- Navigation -->
</template>

<script>
  export default {
  data() {
    return {
      showMobileMenu: false
    }
  }
}
</script>

<style lang="scss" scoped>
  .main__nav, .user__nav {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;

    li {
      display: inline-block;
      margin: 0 10px;
      color: #fff;
      font-size: 16px;
    }
  } // .main__nav, .user__nav

  .user__nav {
    justify-content: flex-end;
  }

  .user__nav--cta {
    border: 2px solid #fff;
    padding: 5px 12px;
    border-radius: 5px;
    line-height: auto;
  }

  .user__nav--login {
    line-height: 38px;
  }

  .logo {
    color: #5359df;
    font-size: 30px;
  }

  .fa-bars, .fa-times {
    color: #5359df;
    width: 60px;
    height: 60px;
    padding: 10px;
    position: relative;
    z-index: 101;
  }

  .mobile__menu--wrapper {
    position: fixed;
    z-index: 100;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgba(255,255,255,0.97);
  }

  .mobile__menu {
    border: 2px solid #5359df;
    border-radius: 15px;
    padding: 20px;
    text-align: center;
    margin: 0;
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    width: 90%;
    list-style: none;
    max-width: 400px;
    li {
      font-size: 18px;
      padding: 10px;
      color: #5359df;
    }
  }// .mobile__menu

  @media all and (max-width: 959px) {
    .main__nav, .user__nav {
      display: none;
    }
  }
</style>

