<template>
  <v-content>
    <v-container fluid class="banner__container">
      <Navbar/>
      <Hero/>
    </v-container>
    <v-container fluid>
      footer
    </v-container>
  </v-content>
</template>

<script>
import Navbar from "~/components/navigation/Navbar"
import Hero from "~/components/navigation/Hero"

export default {
  layout: 'home',
  components: {
    Navbar, Hero
  }
}
</script>

<style lang="scss" scoped>

  .banner__container {
    background-color: #fff;
    background-image: url('/home/home_banner.jpg');
    background-position: top right;
    background-size: auto;
    background-repeat: no-repeat;
  }

  @media all and (max-width: 1550px) {
    .banner__container {
      background-size: contain;
    }
  }

  @media all and (max-width: 1300px) {
    .banner__container {
      background-size: 60%;
    }
  }

  @media all and (max-width: 959px) {
    .banner__container {
      background: none;
    }
  }
  
</style>
