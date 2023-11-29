<script setup>
import AppHeader from "./components/AppHeader.vue";
import AppCardContainer from "./components/AppCardContainer.vue";
import AppBlueContainer from "./components/AppBlueContainer.vue";
import AppMenuContainer from "./components/AppMenuContainer.vue";
import AppFooter from "./components/AppFooter.vue";
</script>

<template>
  <AppHeader />
  <main>
    <AppCardContainer />
    <AppBlueContainer />
    <AppMenuContainer />
  </main>
  <footer>
    <AppFooter />
  </footer>
</template>

<style scoped></style>
