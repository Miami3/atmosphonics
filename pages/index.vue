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
      <no-ssr placeholder="loading...">
        <Applications/>
      </no-ssr>
      <Whythebest/>
      <no-ssr placeholder="loading...">  
        <Testimonials/>
      </no-ssr>
    </v-container>
    <v-container fluid>
      <Footer/>
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
import Whythebest from "~/components/home-sections/whythebest"
import Footer from "~/components/footer"

export default {
  layout: 'home',
  components: {
    Navbar, Hero, MainCTA, Features, Solutions, Services, Whythebest,
    Footer,
    Testimonials: () => import('~/components/home-sections/testimonials'),
    Applications: () => import('~/components/home-sections/applications'),
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
