<template>
    <v-layout row wrap class="features__container">
        <v-flex xs12 md4 class="features__item--wrapper">
            <div class="features__item">
                <img src="/home/project-management.png" alt="Project Management" class="features__item--image">
                <h3 class="features__item--title">Project Management</h3>
                <p class="features__item--text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Aliquam
                    delectus nam iste iusto illo ut eligendi nemo velit, nostrum aspernatur incidunt reprehenderit
                    magnam alias, possimus suscipit quae asperiores facilis blanditiis!
                </p>
                <a href="#" class="features__item--cta">Learn More</a>
            </div>
        </v-flex>
        <v-flex xs12 md4 class="features__item--wrapper">
            <div class="features__item">
                <img src="/home/project-analysis.png" alt="Project Analysis" class="features__item--image">
                <h3 class="features__item--title">Project Analysis</h3>
                <p class="features__item--text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Aliquam
                    delectus nam iste iusto illo ut eligendi nemo velit, nostrum aspernatur incidunt reprehenderit
                    magnam alias, possimus suscipit quae asperiores facilis blanditiis!
                </p>
                <a href="#" class="features__item--cta">Learn More</a>
            </div>
        </v-flex>
        <v-flex xs12 md4 class="features__item--wrapper">
            <div class="features__item">
                <img src="/home/project-management.png" alt="Project Management" class="features__item--image">
                <h3 class="features__item--title">Project Management</h3>
                <p class="features__item--text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Aliquam
                    delectus nam iste iusto illo ut eligendi nemo velit, nostrum aspernatur incidunt reprehenderit
                    magnam alias, possimus suscipit quae asperiores facilis blanditiis!
                </p>
                <a href="#" class="features__item--cta">Learn More</a>
            </div>
        </v-flex>
    </v-layout>
</template>

<style lang="scss" scoped>
.features__container {
    background-color: #f8f8fe;
    padding: 0 0 80px 0;
}
.features__item--wrapper {
    padding: 80px 20px 0 20px;
}
.features__item {
    text-align: center;
}
.features__item--title {
    color: #2c2255;
    font-size: 24px;
    font-weight: normal;
    margin: 40px 0 15px 0;
}
.features__item--text {
    font-size: 18px;
    color: #5c5c5c;
    padding: 0 10px;
}
.features__item--cta {
    display: inline-block;
    margin: 20px 0 0 0;
    color: #3d3d3d;
    font-size: 16px;
    font-weight: 400;
    border: 1px solid #dfdfe4;
    border-radius: 4px;
    text-decoration: none;
    text-align: center;
    padding: 11px 30px 10px 30px;
    transition: all 0.3s ease;

    &:hover {
        background-color: #3d3d3d;
        color: #fff;
    }
}
</style>

