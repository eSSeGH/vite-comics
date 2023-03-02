<script>
export default {
    data() {
        return {
            title: '',
            footerLinks: [],
        }
    },
    props: {
        title: {
            type: String,
            required: true
        },
        footerLinks: {
            type: Array,
            required: true
        }
    }
}
</script>

<template>
    <div>
        <h3>{{ title }}</h3>

        <ul>
            <li v-for="(link, i) in footerLinks" :key="i">
                <a href="">{{ link }}</a>
            </li>
        </ul>

    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors' as *;

.link-footer {
    background-image: url(/img/footer-bg.jpg);
    height: 372px;
    position: relative;
    overflow-y: hidden;

    .container2 {
        width: 30%;
        display: flex;
        gap: 28px;

        .col {
            flex-basis: calc(100% - 28px*2/3);

            h3 {
                color: white;
                font-size: 1.2rem;
                padding: 20px 0;
            }

            ul {
                display: flex;
                flex-direction: column;
                gap: 5px;

                li {

                    a {
                        color: lightgrey;
                        font-size: 0.75rem;

                        &:hover {
                            color: white;
                            text-decoration: underline;
                        }
                    }
                }
            }
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