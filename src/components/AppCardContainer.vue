<script>
import AppCard from "./AppCard.vue";
export default {
  name: "AppCardContainer",
  props: ["comics"],
  components: {
    AppCard,
  },
};
</script>

<template>
  <div class="my-container">
    <div class="container">
      <div class="row">
          <AppCard v-for="comic in comics" :comic="comic" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.my-container {
  background-color: #1c1c1c;
  color: white;
}
</style>
