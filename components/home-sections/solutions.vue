<template>
    <v-layout row wrap class="solutions__container">
      <v-flex xs12 md6 lg5 class="solutions__section">
        <h3 class="solutions__title">We Offer Quick & Powerful <br> Business Solution</h3>
        <ul class="solutions__list">
          <li class="solutions__item">
            <h4 class="solutions__item--title">Clean & Beautifull Interface Layout</h4>
            <p class="solutions__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Cumque dolore et ex id illo impedit molestiae natus nemo odio quam, quas quia ratione reiciendis
              repellat sapiente sunt velit. Optio, sed.
            </p>
          </li>
          <li class="solutions__item">
            <h4 class="solutions__item--title">Easy to Customize your Design</h4>
            <p class="solutions__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Cumque dolore et ex id illo impedit molestiae natus nemo odio quam, quas quia ratione reiciendis
              repellat sapiente sunt velit. Optio, sed.
            </p>
          </li>
          <li class="solutions__item">
            <h4 class="solutions__item--title">Drag & Drop Your Design Here</h4>
            <p class="solutions__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Cumque dolore et ex id illo impedit molestiae natus nemo odio quam, quas quia ratione reiciendis
              repellat sapiente sunt velit. Optio, sed.
            </p>
          </li>
        </ul>
      </v-flex>
      <v-flex xs12 md6 lg7 align-self-center class="solutions__section">
        <img src="/home/devices.png" alt="devices" class="solutions__image">
      </v-flex>
    </v-layout>
</template>

<script>
    export default {
        name: "solutions"
    }
</script>

<style lang="scss" scoped>
  .solutions__container {
    padding: 80px 10px;
    background-color: #fff;
  }
  .solutions__section {
    padding: 0 15px;
  }
  .solutions__title {
    position: relative;
    color: #2c2255;
    font-size: 42px;
    font-weight: 400;
    margin: 0 0 70px 0;
    &:after {
      display: block;
      content: '';
      position: absolute;
      bottom: -15px;
      left: 2px;
      width: 70px;
      height: 2px;
      background-color: #2c2255;
    }
  } // .solutions__title

  .solutions__list {
    list-style: none;
    padding: 0;
  }

  .solutions__item {
    position: relative;
    padding: 0 0 35px 50px;

    &:after {
      display: block;
      content: '';
      position: absolute;
      top: 7px;
      left: 0;
      width: 25px;
      height: 25px;
      background-image: url('/home/check.png');
    }
  }

  .solutions__item--title {
    font-size: 24px;
    color: #2c2255;
    font-weight: 400;
    margin: 0 0 15px 0;
  }

  .solutions__item--text {
    color: #7b7c93;
    font-size: 20px;
  }

  .solutions__image {
    display: block;
    margin: 0 auto;
    width: 100%;
    max-width: 800px;
    height: auto;
  }

  @media all and (max-width: 1350px) {
    .solutions__title {
      font-size: 32px;
    }
    .solutions__item--title {
      font-size: 20px;
    }
    .solutions__item--text {
      font-size: 16px;
    }
  }
</style>
