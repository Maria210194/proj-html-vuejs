<template>
  <div class="container-fluid w-100 d-flex">
    <div class="firstFooter col-3">
      <img src="@/assets/images/footer-logo.png" alt="" />
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatibus
        magnam voluptatem quis reiciendis itaque sint eveniet natus impedit
        eaque, a hic non.
      </p>
      <button class="btn-orange">Learn more</button>
    </div>
    <div class="title-Props d-flex">
      <h5 v-for="(element, index) in link" :key="index">
        {{ element.name }}
      </h5>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
  props: {
    link: Array,
  },
};
</script>

<style lang="scss" scoped>
.container-fluid {
  background-color: #31312f;
  color: #6b6868;
  margin-top: 30px;
  .btn-orange {
    text-transform: uppercase;
  }
  .firstFooter {
    padding: 20px;
    img {
      width: 70%;
      padding: 10px 0;
    }
    p {
      padding: 10px 0;
      margin: 0 auto;
      font-size: 12px;
    }
    button {
      margin: 0 0 10px;
    }
  }
}
</style>