<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<template>
    <section class="subscription-bar">

        <div class="container flex-center">

            <button class="sign-up-btn">
                SIGN-UP NOW!
            </button>

            <div class="follow-us flex-center">
                <span>
                    FOLLOW US
                </span>

                <ul class="flex-center">
                    <li>
                        <a href="">
                            <img src="/img/footer-facebook.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="/img/footer-twitter.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="/img/footer-youtube.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="/img/footer-pinterest.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="/img/footer-periscope.png" alt="">
                        </a>
                    </li>
                </ul>

            </div>

        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors' as *;

.subscription-bar {
    padding: 25px;
    background-color: $dark-grey;

    .container {
        justify-content: space-between;

        .sign-up-btn {
            border: 2px solid $subscription-blue;
            color: $subscription-blue;
            font-size: 14px;
            padding: 18px;
            background-color: $dark-grey;
            transition: transform 300ms;

            &:hover {
                transform: scale(1.2);
            }
        }

        .follow-us {
            gap: 30px;

            span {
                font-size: 18px;
                color: $subscription-blue;
            }

            ul {
                gap: 20px;

                li {

                    a {
                        height: 35px;
                        aspect-ratio: 1;

                        img {
                            transition: transform 300ms;

                            &:hover {
                                transform: scale(1.2);
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>