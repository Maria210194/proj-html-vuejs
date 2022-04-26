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
      <div class="col-7 header-nav">
        <ul>
          <li v-for="element in arrayNav" :key="element">
            <a href="#">{{ element }}</a>
          </li>
        </ul>
      </div>
      <div class="col-2">
        <button class="btn-orange">GET QUOTE!</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      arrayNav: ["HOME", "ABOUT", "SERVICES", "WORK", "ARTICLES"],
    };
  },
};
</script>

<style lang="scss" scoped>
.container-fluid {
  padding: 0;
}
.img-logo {
  width: 170px;
  padding: 10px;
}
.header-nav ul {
  display: flex;
  justify-content: flex-end;
  margin-top: 20px;
}

.header-nav li {
  list-style: none;
  flex: 0 0 auto;
  margin: 15px;

  a {
    color: #666;
    text-decoration: none;
    font-size: 8px;
  }
  &:hover {
    color: #fed23f;
    border-bottom: 2px solid #fed23f;
  }
}
.btn-orange {
  margin-top: 37px;
}
</style>