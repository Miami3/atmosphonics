<template>
  <v-content>
    <v-container fluid class="banner__container">
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
            <li>Login</li>
            <li class="user__nav--cta">Join Now</li>
          </ul>
        </v-flex>
      </v-layout> <!-- Navigation -->
      <v-layout class="hero__container">
        <v-flex xs12 sm6>
            <h1 class="hero__title">
              We Help You to Get <br>
              Best Business Solutions Ever
            </h1>
            <p class="hero__text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab accusamus facilis incidunt
              inventore nam suscipit velit veniam voluptatibus! Ex facilis illo neque obcaecati quae! Deserunt necessitatibus
              nesciunt omnis sequi sint!
            </p>
            <a href="#" class="hero__cta">Get Started Now</a>
        </v-flex>
        <v-flex xs12 sm6>
          <div class="hero__img--wrapper">
            <img src="/home/hero_img.jpeg" alt="team" class="hero__img">
            <img src="/home/play_btn.png" alt="play  button" class="hero__play">
          </div>
        </v-flex>
      </v-layout> <!-- Hero Container -->
    </v-container>
    <v-container fluid>
      footer
    </v-container>
  </v-content>
</template>

<script>
export default {
  layout: 'home'
}
</script>

<style lang="scss" scoped>

  .banner__container {
    background-color: #fff;
    background-image: url('/home/home_banner.jpg');
    background-position: top right;
    background-size: contain;
    background-repeat: no-repeat;
  }

  .hero__img {
    width: 100%;
  }

  .main__nav, .user__nav {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;

    li {
      display: inline-block;
      margin: 0 10px;
    }
  }

  .user__nav {
    justify-content: flex-end;
  }

  .hero__img--wrapper {
    position: relative;
  }

  .hero__play {
    position: absolute;
    z-index: 1;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    transition: all 0.5s ease;

    &:hover {
      cursor: pointer;
    }
  }
</style>
