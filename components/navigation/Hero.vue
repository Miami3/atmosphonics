<template>
    <v-layout row wrap class="hero__container">
        <v-flex xs12 md5 order-xs2 order-md1 class="text-xs-center text-md-left">
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
        <v-flex xs12 md7 order-xs1 order-md2>
          <div class="hero__img--wrapper">
            <img src="/home/hero_img.jpeg" alt="team" class="hero__img">
            <img src="/home/play_btn.png" alt="play  button" class="hero__play">
          </div>
        </v-flex>
      </v-layout> <!-- Hero Container -->
</template>

<style lang="scss" scoped>
    .hero__container {
    padding: 80px 0;
  }

  .hero__title {
    color: #2c2255;
    font-size: 40px;
    font-weight: normal;
    padding: 0 30px 0 0;
  }

  .hero__text {
    color: #7b7c93;
    font-size: 16px;
    padding: 0 50px 0 0;
  }

  .hero__cta {
    display: inline-block;
    text-align: center;
    color: #fff;
    font-size: 20px;
    font-weight: 500;
    padding: 10px 35px;
    background-color: #fd8917;
    text-decoration: none;
    border: 2px solid #fd8917;
    border-radius: 5px;
    margin: 50px 0;
    transition: all 0.4s ease;
    &:hover {
      color: #fd8917;
      background-color: #fff;
    }
  }// .hero__cta

  .hero__img--wrapper {
    position: relative;
    text-align: center;
  }

  .hero__img {
    border-radius: 7px;
    width: 100%;
    max-width: 600px;
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

  @media all and (max-width: 960px) {
    .hero__cta {
        margin: 20px auto;
    }
    .hero__text {
        padding: 0;
        margin: 0;
    }
    .hero__title {
        padding: 0;
        margin: 30px 0 0 0;
        font-size: 32px;
    }
  }
</style>

