<template>
    <v-layout column wrap class="text-xs-center testimonials__container">
        <h2 class="testimonials__section--title">What Our Clients Say ?</h2>
        <p class="testimonials__section--subheader">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Voluptate neque, pariatur culpa nulla alias tempore, tenetur nihil voluptatum quibusdam quam
        </p>
        <div class="carousel__wrapper">
        <carousel :loop="true" :autoplay="true" :autoplayTimeout="3000" :autoplayHoverPause="true" 
            :perPage="5" :perPageCustom="[[100, 1], [600, 2], [960, 3], [1264, 4]]">
            <slide v-for="(item, i) in feedbacks" :key="i" :index="i" class="testimonials__slide">
                <div class="item__wrapper">
                    <img :src="item.avatar" :alt="item.name" class="item__img">
                    <h4 class="item__title">{{ item.name }}</h4>
                    <p class="item__role">{{ item.role }}</p>
                    <p class="item__text">{{ item.text }}</p>
                </div>
            </slide>
        </carousel>
        </div>
    </v-layout>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
    data() {
        return {
          feedbacks: [
              {
                  avatar: './testimonials/barry-holt.jpg',
                  name: 'Barry Holt',
                  role: 'Designer',
                  text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form.'  
              },
              {
                  avatar: './testimonials/martha-gordon.jpg',
                  name: 'Martha Gordon',
                  role: 'HR manager',
                  text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form.'  
              },
              {
                  avatar: './testimonials/charlie-evans.jpg',
                  name: 'Charlie Evans',
                  role: 'Artist',
                  text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form.'  
              },
              {
                  avatar: './testimonials/jacob-neal.jpg',
                  name: 'Jacob Neal',
                  role: 'Engineer',
                  text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form.'  
              },
              {
                  avatar: './testimonials/lia-mccormick.jpg',
                  name: 'Lia Kanter',
                  role: 'Digital Nomad',
                  text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form.'  
              },
              {
                  avatar: './testimonials/naomi-smith.jpg',
                  name: 'Naomi Smith',
                  role: 'Scientist',
                  text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form.'  
              }
          ]
        }
    },
    components: { Carousel, Slide }
}
</script>

<style lang="scss" scoped>
.testimonials__container {
    padding: 80px 10px;
    background-color: #fff;
}
.testimonials__section--title {
    color: #2c2255;
    font-size: 42px;
    font-weight: normal;

}
.testimonials__section--subheader {
    color: #7b7c93;
    font-size: 20px;
    font-weight: normal;
    margin: 0 auto;
    max-width: 700px;
}

.carousel__wrapper {
    padding: 50px 0 0 0;
}

.testimonials__slide {
    padding: 25px;
}

.item__wrapper {
    border-bottom: 4px solid #5359df;
    background-color: #fff;
    border-radius: 4px;
    box-shadow: 0px 0px 5px 1px rgba(0,0,0,0.3);
    padding: 20px;
    text-align: left;
    max-width: 280px;
    margin: 0 auto;
}

.item__img {
    border-radius: 50%;
    margin: 20px;
}

.item__title {
    font-size: 24px;
    color: #2c2255;
    font-weight: normal;
}

.item__role, .item__text {
    font-size: 18px;
    color: #7b7c93;
}

@media all and (max-width: 650px) {
    .testimonials__section--title {
        font-size: 28px;
    }
    .testimonials__section--subheader {
        font-size: 16px;
    }
}
</style>
