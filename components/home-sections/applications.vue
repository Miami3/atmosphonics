<template>
    <v-layout column wrap class="text-xs-center applications__container">
        <h2 class="applications__section--title">Applications Screenshots</h2>
        <p class="applications__section--subheader">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Voluptate neque, pariatur culpa nulla alias tempore, tenetur nihil voluptatum quibusdam quam
        </p>
        <div class="applications__carousel--wrapper">
        <carousel-3d :autoplay="true" :autoplayTimeout="3500" :autoplayHoverPause="true" :dir="'ltr'">
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
        </div>
    </v-layout>
</template>

<script>
import { Carousel3d, Slide } from 'vue-carousel-3d';

export default {
    components: { Carousel3d, Slide }
}
</script>

<style lang="scss" scoped>
.applications__container {
    padding: 80px 10px;
    background-color: #fff;
}
.applications__section--title {
    color: #2c2255;
    font-size: 42px;
    font-weight: normal;

}
.applications__section--subheader {
    color: #7b7c93;
    font-size: 20px;
    font-weight: normal;
    margin: 0 auto;
    max-width: 700px;
}
.applications__carousel--wrapper {
    margin:  50px 0 0 0;
}
.applications__slide--image {
    height: 100%;
}
.carousel-3d-slide {
    border: none;
}
@media all and (max-width: 650px) {
    .applications__section--title {
        font-size: 28px;
    }
    .applications__section--subheader {
        font-size: 16px;
    }
}
</style>
