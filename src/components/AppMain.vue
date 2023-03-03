<script>
import MainCard from './MainCard.vue'
export default {
    components: {
        MainCard,
    },
    data() {
        return {
            cards: [{
                thumb: "/img/images.png",
                price: "$19.99",
                series: "Action Comics",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$3.99",
                series: "American Vampire 1976",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$16.99",
                series: "Aquaman",
                type: "graphic novel"
            },
            {
                thumb: "/img/images.png",
                price: "$2.99",
                series: "Batgirl",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$3.99",
                series: "Batman",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$2.99",
                series: "Batman Beyond",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$3.99",
                series: "Batman/Superman",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$4.99",
                series: "Batman/Superman Annual",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$5.99",
                series: "Batman: The Joker War Zone",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$6.99",
                series: "Batman: Three Jokers",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$4.99",
                series: "Batman: White Knight Presents: Harley Quinn",
                type: "comic book"
            },
            {
                thumb: "/img/images.png",
                price: "$16.99",
                series: "Catwoman",
                type: "graphic novel"
            }]
        }
    }
}
</script>

<template>
    <main>

        <div class="black-section">

            <div class="container">

                <div class="row">

                    <MainCard class="col" v-for="(card, i) in cards" :key="i" :card="card" />

                </div>

            </div>

        </div>

    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors' as *;

main {
    background-image: url(/img/jumbotron.jpg);
    padding-top: 400px;

    .black-section {
        background-color: $black;

        .container {
            width: 1280px;
            padding: 55px 0;

            .row {
                display: flex;
                flex-wrap: wrap;
                gap: 28px;


                .col {
                    width: calc(100%/6 - 28px*5/6);
                }
            }
        }
    }
}
</style>