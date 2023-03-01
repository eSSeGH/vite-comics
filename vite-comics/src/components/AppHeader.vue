<script>
export default {

}
</script>

<template>
    <header class="main-header">

        <div class="container flex-center">

            <div class="logo">
                <img src="/img/dc-logo.png" alt="dc logo horizontal">
            </div>

            <nav class="navbar">

                <ul style='display: contents'>
                    <li class="nav-link">
                        <a href="">CHARACTERS</a>
                    </li>
                    <li class="nav-link">
                        <a href="">COMICS</a>
                    </li>
                    <li class="nav-link">
                        <a href="">MOVIES</a>
                    </li>
                    <li class="nav-link">
                        <a href="">TV</a>
                    </li>
                    <li class="nav-link">
                        <a href="">GAMES</a>
                    </li>
                    <li class="nav-link">
                        <a href="">COLLECTIBLES</a>
                    </li>
                    <li class="nav-link">
                        <a href="">VIDEOS</a>
                    </li>
                    <li class="nav-link">
                        <a href="">FANS</a>
                    </li>
                    <li class="nav-link">
                        <a href="">NEWS</a>
                    </li>
                    <li class="nav-link">
                        <a href="">SHOP</a>
                    </li>
                </ul>

            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors';

.main-header {
    background-color: white;
    height: 120px;

    .container {
        height: 100%;
        margin: 0 auto;
        justify-content: space-between;

        .logo {
            height: 82px;
            aspect-ratio: 1;
        }

        .navbar {
            height: 100%;
            display: flex;
            gap: 32px;

            .nav-link {
                height: 100%;
                color: $black;
                font-size: 0.75rem;
                font-weight: 500;

                &:active {
                    border-bottom: 5px solid $blue;
                }
            }
        }
    }
}
</style>