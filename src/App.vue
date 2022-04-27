<template>
  <div id="app">
    <HeaderComponent :links="arrayNav" />
    <MainComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import arrayNav from "@/assets/data/arrayNav";

export default {
  name: "App",
  data() {
    return { arrayNav };
  },
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
};
</script>

<style lang="scss">
@import "@/assets/style/generals";
</style>
