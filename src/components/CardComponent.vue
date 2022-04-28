<template>
  <div class="card col-3">
    <i class="fa-solid fa-house"></i>
    <h5>{{ card.title }}</h5>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis
      reprehenderit repudiandae voluptatibus vel aut molestias sequi.
    </p>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props: {
    card: Object,
  },
};
</script>

<style lang="scss" scoped>
.card {
  padding: 10px;
  text-align: center;
  color: #6b6868;
  background-color: #f5f5f5;
  font-size: 10px;
  margin: 0 10px;
  &:hover {
    background-color: #fed23f;
    color: #6b6868;
  }

  i {
    font-size: 20px;
    padding: 10px;
    border-radius: 50%;
    border: 1px solid #6b6868;
  }
}
</style>