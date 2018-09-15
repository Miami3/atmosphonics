<template>
  <v-content>
    <v-container fluid>
      <v-layout>
        <nav class="navigation">

        </nav>
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
            <img src="/home/macbook.png" alt="macbook" class="hero__img">
          </v-flex>
        </v-layout>
      </v-layout>
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

<style scoped>
  .hero__img {
    width: 100%;
  }
</style>
