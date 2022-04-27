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
    <div class="card-container w-90 d-flex">
      <div class="info col-8">
        <h4>Specialist in Modern Costruction</h4>
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cumque nemo
          illo amet nam cupiditate sed eveniet voluptatem assumenda tempora
          nostrum.
        </p>
      </div>
      <div id="cards">
        <div class="card col-3">
          <i class="fa-regular fa-building"></i>
          <h5>Buildings</h5>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis
            reprehenderit repudiandae voluptatibus vel aut molestias sequi.
          </p>
        </div>
        <div class="card col-3">
          <i class="fa-solid fa-recycle"></i>
          <h5>Renovate</h5>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis
            reprehenderit repudiandae voluptatibus vel aut molestias sequi.
          </p>
        </div>
        <div class="card col-3">
          <i class="fa-solid fa-house"></i>
          <h5>Construct</h5>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis
            reprehenderit repudiandae voluptatibus vel aut molestias sequi.
          </p>
        </div>
        <div class="card col-3">
          <i class="fa-solid fa-truck"></i>
          <h5>Exclusive</h5>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis
            reprehenderit repudiandae voluptatibus vel aut molestias sequi.
          </p>
        </div>
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
.card-container {
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
  #cards {
    flex-direction: row;
  }
}
</style>