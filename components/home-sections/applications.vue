<template>
    <v-layout row wrap class="applications__container">
        <h2 class="applications__section--title">Applications Screenshots</h2>
        <p class="applications__section--subheader">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Voluptate neque, pariatur culpa nulla alias tempore, tenetur nihil voluptatum quibusdam quam
            ipsam deleniti repellat provident et dolor, ab nobis dolorem illum?
        </p>
        <carousel-3d>
            <slide :index="0">
                <img src="~/static/3d/apple.jpg" alt="apple" class="applications__slide--image">
            </slide>
            <slide :index="1">
                <img src="~/static/3d/planning.jpg" alt="planning" class="applications__slide--image">
            </slide>
            <slide :index="2">
                <img src="~/static/3d/server.jpg" alt="planning" class="applications__slide--image">
            </slide>
            <slide :index="3">
                <img src="~/static/3d/startup.jpg" alt="startup" class="applications__slide--image">
            </slide>
            <slide :index="4">
                <img src="~/static/3d/code.jpg" alt="code" class="applications__slide--image">
            </slide>
        </carousel-3d>
    </v-layout>
</template>

<script>
import { Carousel3d, Slide } from 'vue-carousel-3d';

export default {
    components: { Carousel3d, Slide }
}
</script>

<style lang="scss" scoped>

</style>
