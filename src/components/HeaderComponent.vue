<template>
  <div class="container-fluid w-90">
    <div class="d-flex row">
      <div class="col-3">
        <img
          class="img-logo"
          src="@/assets/images/construction_logo_retina.png"
          alt="logo_img"
        />
      </div>
      <div class="col-9 header-nav"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style lang="scss" scoped>
.img-logo {
  width: 100px;
}
</style>