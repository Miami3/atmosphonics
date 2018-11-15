<template>
    <v-layout column align-center class="maincta__wrapper">
        <h2 class="maincta__title">Overall 1200 happy client, Get start Now</h2>
        <p class="maincta__subtitle">Lorem ipsum dolor sit amet consectetur adipisicing
            elit. Nostrum ipsam rerum amet illo voluptatibus provident similique,
            tempore totam atque? Ut suscipit est minima repudiandae amet illo optio,
            ex at! Unde?
        </p>
        <div class="maincta__buttons--wrapper">
            <button class="maincta__button">Join Now</button>
            <button class="maincta__button blue__btn">Start A Free Trial</button>
        </div>
    </v-layout>
</template>

<style lang="scss" scoped>
.maincta__wrapper {
    padding: 50px 80px;
}
.maincta__title {
    color: #2c2255;
    font-size: 40px;
    font-weight: normal;
    text-align: center;
}
.maincta__subtitle {
    color: #7b7c93;
    font-size: 16px;
    text-align: center;
    max-width: 800px;
    padding: 15px 0 40px 0;
}
.maincta__buttons--wrapper {
    text-align: center;
}
.maincta__button {
    display: inline-block;
    text-align: center;
    color: #fff;
    font-size: 20px;
    font-weight: 500;
    padding: 10px 35px;
    background-color: #fd8917;
    text-decoration: none;
    border: 2px solid #fd8917;
    border-radius: 5px;
    margin: 10px;
    transition: all 0.4s ease;
    &:hover {
      color: #fd8917;
      background-color: #fff;
    }

    &.blue__btn {
        background-color: #5359df;
        border: 2px solid #5359df;
        &:hover {
            color: #5359df;
            background-color: #fff;
        }
    }
}
@media all and (max-width: 960px) {
    .maincta__wrapper {
    padding: 50px 0;
}
}
</style>

