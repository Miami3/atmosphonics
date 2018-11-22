<template>
    <v-layout row wrap class="solutions__container">
      <v-flex xs12 md6 lg5 class="solutions__section">
        <h3 class="solutions__title">Why we are the best &<br>Customers Choose Us ?</h3>
        <ul class="solutions__list">
          <li class="solutions__item">
            <h4 class="solutions__item--title">Clean & Beautifull Interface Layout</h4>
            <p class="solutions__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
          </li>
          <li class="solutions__item">
            <h4 class="solutions__item--title">Easy to Customize your Design</h4>
            <p class="solutions__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
          </li>
          <li class="solutions__item">
            <h4 class="solutions__item--title">Drag & Drop Your Design Here</h4>
            <p class="solutions__item--text">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
          </li>
        </ul>
      </v-flex>
      <v-flex xs12 md6 lg7 align-self-center class="solutions__section">
        <iframe class="solutions__video" src="https://www.youtube.com/embed/2L0ZHxcoWhM" frameborder="0"
         allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </v-flex>
    </v-layout>
</template>

<script>
    export default {
        name: "whythebest"
    }
</script>

<style lang="scss" scoped>
  .solutions__container {
    padding: 80px 10px;
    background-color: #f6f7fd;
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

  .solutions__video {
    width: 100%;
    height: 500px;
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
  @media all and (max-width: 1150px) {
    .solutions__video {
      height: 450px;
    }
  }
  @media all and (max-width: 900px) {
    .solutions__video {
      height: 400px;
    }
  }
  @media all and (max-width: 600px) {
    .solutions__video {
      height: 300px;
    }
  }
</style>