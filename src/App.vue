<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppJumbotron from "./components/AppJumbotron.vue"
export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppJumbotron,
  }
}
</script>

<template>
  <AppHeader></AppHeader>

  <AppJumbotron></AppJumbotron>

  <AppMain></AppMain>

  <AppFooter></AppFooter>

 
</template>

<style></style>
