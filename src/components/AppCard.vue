<script>
export default {
  props: {
    comic: Object
  },
};
</script>

<template>
  <div class="my-card col-2 my-4">
    <img :src="comic.thumb" alt="" />
    <h3>{{ comic.series }}</h3>
  </div>
</template>

<style scoped>
.my-card img{
  width: 10rem;
  height: 10rem;
}

h3{
  font-size: 1rem;
  text-wrap: wrap;
}
</style>
