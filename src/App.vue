<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppMarketing from './components/AppMarketing.vue'
import AppLinks from './components/AppLinks.vue'
import AppSubscription from './components/AppSubscription.vue'
import "@fontsource/roboto-condensed"

export default {
  components: {
    AppHeader,
    AppMain,
    AppMarketing,
    AppLinks,
    AppSubscription,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppMarketing />
  <AppLinks />
  <AppSubscription />
</template>

<style scoped></style>
