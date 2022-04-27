<template>
  <div id="app">
    <HeaderComponent :links="arrayNav" />
    <MainComponent :iconCard="iconCard" />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import arrayNav from "@/assets/data/arrayNav";

import iconCard from "@/assets/data/iconCard";

export default {
  name: "App",
  data() {
    return {
      iconCard,
      arrayNav,
    };
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
