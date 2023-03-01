<script>
export default {

}
</script>

<template>
    <main>

        <div class="container">

            <div class="content">
                --> CONTENT GOES HERE &lt;-- </div>

        </div>

    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/colors' as *;

main {
    background-color: black;
    padding: 52px 0;

    .content {
        color: white;
    }
}
</style>