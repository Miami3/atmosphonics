<template>
  <v-content>
    <v-container fluid class="banner__container">
      <Navbar/>
      <Hero/>
      <no-ssr placeholder="loading...">
        <Tech/>
      </no-ssr>
    </v-container>
    <v-container fluid pa-0>
      <main-c-t-a/>
      <Features/>
      <Solutions/>
      <Services/>  
    </v-container>
    <v-container fluid>
      footer
    </v-container>
  </v-content>
</template>

<script>
import Navbar from "~/components/navigation/Navbar"
import Hero from "~/components/navigation/Hero"
import MainCTA from "~/components/home-sections/main-cta"
import Features from "~/components/home-sections/features"
import Solutions from "~/components/home-sections/solutions"
import Services from "~/components/home-sections/services"

export default {
  layout: 'home',
  components: {
    Navbar, Hero, MainCTA, Features, Solutions, Services,
    Tech: () => import('~/components/tech/Technologies')
  }
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

  .no__padding {
    padding: 0;
  }

  @media all and (max-width: 1550px) {
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
