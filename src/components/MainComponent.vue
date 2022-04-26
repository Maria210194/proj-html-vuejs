<template>
  <div class="container-fluid">
    <div class="top-jumbo w-100 d-flex">
      <h3>Building ispiring spaces</h3>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
      <div class="btn">
        <button class="btn-black">EXPLORE RECENT WORK</button>
        <button class="btn-orange">GET QUOTE TODAY!</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style lang="scss" scoped>
.container-fluid {
  padding: 0;
}
.top-jumbo {
  flex-direction: column;
  justify-content: center;
  height: 400px;
  background-image: url(@/assets/images/home-slider-62528242.jpg);
  background-position: center;
  background-size: cover;
  h3 {
    color: white;
    text-transform: uppercase;
  }
  p {
    color: #fed23f;
  }
  button {
    margin: 10px;
  }
}
</style>