<script>
export default {

}
</script>

<template>
    <section class="marketing">

        <div class="container">

            <div class="marketing-cards flex-center">

                <ul style="display: contents;">
                    <li class="card flex-center">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </li>
                    <li class="card flex-center">
                        <img src="/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </li>
                    <li class="card flex-center">
                        <img src="/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </li>
                    <li class="card flex-center">
                        <img src="/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </li>
                    <li class="card flex-center">
                        <img src="/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </li>
                </ul>

            </div>

        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors' as *;

.marketing {
    background-color: $blue;
    padding: 52px 0;

    .marketing-cards {
        justify-content: space-around;

        .card {

            img {
                height: 60px;
            }

            span {
                color: white;
                font-size: 1rem;
            }
        }
    }
}
</style>