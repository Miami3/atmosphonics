<template>
    <v-layout row wrap class="services__container">
        <v-flex xs12 class="services__header--wrapper">
            <h3 class="services__header--title">Our Application Core Features</h3>
            <p class="services__header--text">Lorem ipsum dolor sit amet consectetur adipisicing
                elit. Rerum non, veritatis cum laudantium iure sit, voluptatem animi sequi explicabo.
            </p>
        </v-flex>
        <v-flex xs12 md6 lg4 class="services__item--wrapper">
            <div class="services__item">
                <div class="services__image--container">
                    <img src="/services/content-management.png" alt="Content Management" class="services__image">
                </div>
                <h4 class="services__item--title">Content Management</h4>
                <p class="services__item--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                    Optio eaque ullam expedita, non quis voluptate odio cupiditate perferendis atque consectetur
                    eum nisi quam reprehenderit debitis, voluptatibus, mollitia ex facere ratione!
                </p>
            </div>
        </v-flex>
        <v-flex xs12 md6 lg4 class="services__item--wrapper">
            <div class="services__item">
                <div class="services__image--container">
                    <img src="/services/project-analysis.png" alt="Project Analysis" class="services__image">
                </div>
                <h4 class="services__item--title">Project Analysis</h4>
                <p class="services__item--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                    Optio eaque ullam expedita, non quis voluptate odio cupiditate perferendis atque consectetur
                    eum nisi quam reprehenderit debitis, voluptatibus, mollitia ex facere ratione!
                </p>
            </div>
        </v-flex>
        <v-flex xs12 md6 lg4 class="services__item--wrapper">
            <div class="services__item">
                <div class="services__image--container">
                    <img src="/services/support.png" alt="Support & Service" class="services__image">
                </div>
                <h4 class="services__item--title">Support & Service</h4>
                <p class="services__item--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                    Optio eaque ullam expedita, non quis voluptate odio cupiditate perferendis atque consectetur
                    eum nisi quam reprehenderit debitis, voluptatibus, mollitia ex facere ratione!
                </p>
            </div>
        </v-flex>
        <v-flex xs12 md6 lg4 class="services__item--wrapper">
            <div class="services__item">
                <div class="services__image--container">
                    <img src="/services/project-management.png" alt="Project Management" class="services__image">
                </div>
                <h4 class="services__item--title">Project Management</h4>
                <p class="services__item--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                    Optio eaque ullam expedita, non quis voluptate odio cupiditate perferendis atque consectetur
                    eum nisi quam reprehenderit debitis, voluptatibus, mollitia ex facere ratione!
                </p>
            </div>
        </v-flex>
        <v-flex xs12 md6 lg4 class="services__item--wrapper">
            <div class="services__item">
                <div class="services__image--container">
                    <img src="/services/free-updates.png" alt="Get Free Update" class="services__image">
                </div>
                <h4 class="services__item--title">Get Free Update</h4>
                <p class="services__item--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                    Optio eaque ullam expedita, non quis voluptate odio cupiditate perferendis atque consectetur
                    eum nisi quam reprehenderit debitis, voluptatibus, mollitia ex facere ratione!
                </p>
            </div>
        </v-flex>
        <v-flex xs12 md6 lg4 class="services__item--wrapper">
            <div class="services__item">
                <div class="services__image--container">
                    <img src="/services/smart-performance.png" alt="Smart Performance" class="services__image">
                </div>
                <h4 class="services__item--title">Smart Performance</h4>
                <p class="services__item--text">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                    Optio eaque ullam expedita, non quis voluptate odio cupiditate perferendis atque consectetur
                    eum nisi quam reprehenderit debitis, voluptatibus, mollitia ex facere ratione!
                </p>
            </div>
        </v-flex>
    </v-layout>
</template>

<script>
    
</script>

<style lang="scss" scoped>
.services__container {
    padding: 80px 10px;
    background-color: #f6f7fd;
    text-align: center;
}
.services__header--wrapper {
    margin: 0 0 50px 0;
}
.services__header--title {
    font-size: 42px;
    font-weight: normal;
    color: #2c2255;
    padding: 30px 0 20px 0;
}
.services__header--text {
    color: #7b7c93;
    font-size: 20px;
    margin: 0 auto;
    max-width: 800px;
}
.services__item--wrapper {
    padding: 15px 15px 50px 15px;
}
.services__image--container {
    position: relative;
    background-color: rgba(101,104,170, 0.1);
    border-radius: 50%;
    width: 60px;
    height: 60px;
    margin: 0 auto 25px auto;
    transform: translateX(-20px);
}
.services__image {
    display: block;
    position: absolute;
    left: 25px;
    bottom: 20px;
}
.services__item--title {
    color: #3d3d3d;
    font-size: 24px;
    font-weight: normal;
    margin: 0 0 25px 0;
}
.services__item--text {
    color: #5c5c5c;
    font-size: 18px;
    padding: 0 10px;
}
</style>
