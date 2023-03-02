<script>
import AppLinksMenu from './AppLinksMenu.vue'

export default {
    components: {
        AppLinksMenu,
    },
    data() {
        return {}
    }

}
</script>

<template>
    <section class="link-footer">

        <div class="container">

            <div class="container2">

                <div class="col">

                    <AppLinksMenu :title="'DC COMICS'" :footerLinks="[
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News',
                    ]" />

                    <AppLinksMenu :title="'SHOP'" :footerLinks="[
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]" />
                </div>

                <div class="col">

                    <AppLinksMenu :title="'DC'" :footerLinks="[
                        'Terms of use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',
                    ]" />
                </div>

                <div class="col">

                    <AppLinksMenu :title="'SITES'" :footerLinks="[
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]" />
                </div>

            </div>

        </div>

        <img src="/img/dc-logo-bg.png" alt="">

    </section>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors' as *;

.link-footer {
    background-image: url(/img/footer-bg.jpg);
    position: relative;
    overflow-y: hidden;
    padding-bottom: 30px;

    .container2 {
        width: 30%;
        display: flex;
        gap: 28px;

        .col {
            flex-basis: calc(100% - 28px*2/3);
        }
    }

    img {
        height: 563px;
        aspect-ratio: 1;
        position: absolute;
        top: -70px;
        right: 320px;
    }
}
</style>