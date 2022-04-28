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
.info-container .iconsColorate {
  color: red;
  &:hover {
    color: #fed23f;
    background-color: #f5f5f5;
  }
  h5 {
    color: #6b6868;
  }
  p {
    color: #6b6868;
  }
}
.title-Props {
  h5 {
    color: #fed23f;
    font-size: 12px;
    margin: 30px 10px;
  }
}
</style>
