<template>
  <div class="card col-3">
    <i class="card.icon"></i>
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

<style>
</style>