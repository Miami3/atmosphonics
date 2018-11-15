<template>
    <div>
    <carousel :loop="true" :autoplay="true" :autoplayTimeout="3000" :autoplayHoverPause="true" 
    :perPage="5" :perPageCustom="[[100, 1], [600, 2], [960, 3], [1264, 4]]">
        <slide :index="0" class="img__wrapper">
            <img src="/tech/html.png" alt="html" class="item">
        </slide>
        <slide :index="1" class="img__wrapper">
            <img src="/tech/css.png" alt="css" class="item">
        </slide>
        <slide :index="2" class="img__wrapper">
            <img src="/tech/js.png" alt="javascript" class="item">
        </slide>
        <slide :index="3" class="img__wrapper">
            <img src="/tech/mongo.png" alt="mongo" class="item">
        </slide>
        <slide :index="4" class="img__wrapper">
            <img src="/tech/mysql.png" alt="mysql" class="item">
        </slide>
        <slide :index="5" class="img__wrapper">
            <img src="/tech/node.png" alt="node" class="item">
        </slide>
        <slide :index="6" class="img__wrapper">
            <img src="/tech/php.png" alt="php" class="item">
        </slide>
        <slide :index="7" class="img__wrapper">
            <img src="/tech/webpack.png" alt="webpack" class="item">
        </slide>
        <slide :index="8" class="img__wrapper">
            <img src="/tech/vue.png" alt="vue" class="item">
        </slide>
        <slide :index="9" class="img__wrapper">
            <img src="/tech/nuxt.png" alt="nuxt" class="item">
        </slide>
        <slide :index="10" class="img__wrapper">
            <img src="/tech/git.png" alt="git" class="item">
        </slide>
    </carousel>
    </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
    data() {
        return {
          odd: true
        }
    },
    components: { Carousel, Slide }
}
</script>

<style lang="scss" scoped>
    .img__wrapper {
        text-align: center;
        transition: all 0.4s linear;
    }
    
    .item {
        max-width: 100%;
        height: 150px;
        vertical-align: middle;
    }
</style>
