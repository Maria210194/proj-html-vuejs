<template>
  <div id="app">
    <HeaderComponent :links="arrayNav" />
    <MainComponent :iconCard="iconCard" :iconCard2="iconCard2" />
    <FooterComponent :link="arrayFooter" />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

// Data
import arrayNav from "@/assets/data/arrayNav";
import iconCard from "@/assets/data/iconCard";
import iconCard2 from "@/assets/data/iconCard2";
import arrayFooter from "@/assets/data/arrayFooter";

export default {
  name: "App",
  data() {
    return {
      arrayNav,
      iconCard,
      iconCard2,
      arrayFooter,
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
