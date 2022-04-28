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
    <div class="secondSection col-9">
      <div class="title-Props d-flex">
        <h5
          v-for="(element, index) in link"
          :key="index"
          class="single-section col-4"
        >
          {{ element.name }}
        </h5>
      </div>
      <div class="d-flex">
        <div class="infoFooter d-flex col-4">
          <div class="col-2">
            <img
              class="logoFusion"
              src="@/assets/images/3a74ce3d0532b7773b174c45ca3bd05a_normal.png"
              alt=""
            />
          </div>
          <div class="themeFusion col-10">
            <h6>ThemeFusion</h6>
            <p>@ThemeFusion</p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod
              labore quos dolorum, quae doloribus sed earum mollitia fuga nulla
              dolorem sint.
            </p>
            <img src="@/assets/images/En2TRxLW4AEiWUN.jpeg" alt="" />
          </div>
        </div>
        <div class="col-4">
          <div class="infoFooter d-flex">
            <div class="col-1">
              <i class="fa-solid fa-earth-americas contactIcon"></i>
            </div>
            <div class="col-11">
              <p class="fontSmall">
                Corporate Location1600 Amphitheatre Parkway London WC1 1BA
              </p>
            </div>
          </div>
          <div class="infoFooter d-flex">
            <div class="col-1">
              <i class="fa-solid fa-house contactIcon"></i>
            </div>
            <div class="col-11">
              <p class="fontSmall">
                Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA.
              </p>
            </div>
          </div>
          <div class="infoFooter d-flex">
            <div class="col-1">
              <i class="fa-solid fa-phone contactIcon"></i>
            </div>
            <div class="col-11">
              <p class="fontSmall">1.800.458.556 / 1.800.532.2112.</p>
            </div>
          </div>
          <div class="infoFooter d-flex">
            <div class="col-1">
              <i class="fa-regular fa-envelope contactIcon"></i>
            </div>
            <div class="col-11">
              <p class="fontSmall">info@your-domain.com</p>
            </div>
          </div>
          <div class="infoFooter d-flex">
            <div class="col-1">
              <i class="fa-regular fa-clock contactIcon"></i>
            </div>
            <div class="col-11">
              <p class="fontSmall">Monday - Friday: 9:00 AM - 6:00 PM.</p>
            </div>
          </div>
          <div class="infoFooter d-flex">
            <div class="col-1">
              <i class="fa-regular fa-clock contactIcon"></i>
            </div>
            <div class="col-11">
              <p class="fontSmall">Saturday - Sunday: 9:00 AM - 12:00 PM</p>
            </div>
          </div>
        </div>
        <div class="infoFooter mapConteiner col-4">
          <img class="map" src="@/assets/images/map.png" alt="" />
        </div>
      </div>
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
  background-color: #1e1e1e;
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
  .single-section {
    height: fit-content;
  }
  .infoFooter {
    padding: 3px;
    .map {
      width: 190px;
    }
  }
  .logoFusion {
    width: 30px;
    border-radius: 50%;
  }

  .themeFusion {
    h6 {
      padding-top: 5px;
      color: white;
      font-size: 12px;
      margin: 0 auto;
    }
    p {
      font-size: 10px;
      margin: 5px 0 auto;
    }
    img {
      width: 190px;
      border-radius: 0;
    }
  }
  .fontSmall {
    margin: 0;
  }
  .mapConteiner {
    padding: 10px 30px;
  }
  .contactIcon {
    padding: 0 0 3px 3px;
  }
}
</style>