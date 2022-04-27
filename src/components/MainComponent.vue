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
    <div class="bottom-jumbo">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit?</p>
      <button class="btn-black">GET A FREE QUOTE</button>
    </div>
    <div class="info-container w-90 d-flex">
      <div class="info col-8">
        <h4>Specialist in Modern Costruction</h4>
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cumque nemo
          illo amet nam cupiditate sed eveniet voluptatem assumenda tempora
          nostrum.
        </p>
      </div>
    </div>
    <div class="d-flex w-90 ml-0">
      <CardComponent
        v-for="(item, index) in iconCard"
        :key="index"
        :card="item"
      />
    </div>
  </div>
</template>

<script>
import CardComponent from "@/components/CardComponent.vue";

export default {
  name: "MainComponent",
  props: {
    iconCard: Array,
  },
  components: {
    CardComponent,
  },
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

.bottom-jumbo {
  background-color: #fed23f;
  text-align: center;

  p {
    font-size: 18px;
    color: #6b6868;
    padding: 20px 0 5px 0;
    margin: 0;
  }

  .btn-black {
    position: relative;
    top: 10px;
    padding: 5px 15px;
    border: 1px solid #1e1e1e;
    &:hover {
      background-color: white;
      color: #1e1e1e;
    }
  }
}
.info-container {
  flex-direction: column;
  padding-top: 30px;
  text-align: center;
  color: #6b6868;
  p {
    font-size: 10px;
  }
  h4 {
    font-weight: 100;
    font-size: 18px;
  }
}

.ml-0 {
  margin-left: 0;
}

.card {
  padding: 10px;
  text-align: center;
  color: #6b6868;
  background-color: #f5f5f5;
  font-size: 10px;
  margin: 0 10px;
  i {
    font-size: 20px;
    padding: 10px;
    border-radius: 50%;
    border: 1px solid #6b6868;
  }
}
</style>