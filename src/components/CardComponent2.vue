<template>
  <div class="card col-3">
    <i class="fa-solid fa-suitcase"></i>
    <h3>{{ card2.title }}</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
  </div>
</template>

<script>
export default {
  name: "CardComponent2",
  props: {
    card2: Object,
  },
};
</script>

<style lang="scss" scoped>
.card {
  max-width: calc(100% / 5);
  padding: 10px;
  text-align: center;
  color: #fed23f;
  font-size: 10px;
  margin: 30px auto;
  background-color: transparent;
  border: 0;
  p {
    color: white;
  }
  &:hover {
    background-color: #fed23f;
    color: #6b6868;
  }

  i {
    font-size: 25px;
    padding: 10px;
  }
}
</style>