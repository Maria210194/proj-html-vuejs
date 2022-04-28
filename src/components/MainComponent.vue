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
    <div class="imageContainer">
      <div class="col-8 icon2 d-flex ml-0">
        <CardComponent2
          v-for="(item, index) in iconCard2"
          :key="index"
          :card2="item"
        />
      </div>
    </div>
    <div class="info-container w-80 d-flex">
      <div class="col-8">
        <h4>Explore Recent Work</h4>
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cumque nemo
          illo amet nam cupiditate sed eveniet voluptatem assumenda tempora
          nostrum.
        </p>
        <div class="cardImage d-flex">
          <img
            src="@/assets/images/project2-featured-15013609.jpg"
            alt="img1"
          />
          <img
            src="@/assets/images/project1-featured-294276386.jpg"
            alt="img1"
          />
          <img
            src="@/assets/images/project3-featured-189023420.jpg"
            alt="img1"
          />
        </div>
      </div>
    </div>
    <div class="info-container w-80 d-flex">
      <h4>Our Core Values</h4>
      <p class="w-60">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cumque nemo
        illo amet nam cupiditate sed eveniet voluptatem assumenda tempora
        nostrum.
      </p>
      <div class="iconCard d-flex w-60">
        <CardComponent
          v-for="(item, index) in iconCard"
          :key="index"
          :card="item"
          class="iconsColorate"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardComponent from "@/components/CardComponent.vue";
import CardComponent2 from "@/components/CardComponent2.vue";

export default {
  name: "MainComponent",
  props: {
    iconCard: Array,
    iconCard2: Array,
  },
  components: {
    CardComponent,
    CardComponent2,
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
  margin-top: 20px;
  text-align: center;
  color: #6b6868;
  p {
    font-size: 10px;
  }
  h4 {
    width: fit-content;
    padding: 10px;
    font-weight: 100;
    font-size: 18px;
    border-bottom: 1px solid #fed23f;
  }
}

.ml-0 {
  margin-left: 0;
}

.imageContainer {
  margin: 30px 0;
  background-image: url("../assets/images/home-244125289.jpg");
  background-position: center;
  background-size: cover;
  min-height: 200px;
  align-content: center;
  vertical-align: middle;
}
.cardImage {
  margin: 20px 0;
  img {
    width: 30%;
  }
}
.icon2 {
  margin: 0 auto;
}
.iconCard {
  margin: 0 auto;
  margin-left: 50px;
}
</style>