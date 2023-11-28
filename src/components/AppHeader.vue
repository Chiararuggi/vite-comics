<script>
export default {
  name: "AppHeader",
  data() {
    return {
      menuLinks: [
        {
          text: "Characters",
          url: "#characters",
        },
        {
          text: "comics",
          url: "#comics",
        },
        {
          text: "Movies",
          url: "#movies",
        },
        {
          text: "Tv",
          url: "#tv",
        },
        {
          text: "Games",
          url: "#games",
        },
        {
          text: "Collectibles",
          url: "#collectibles",
        },
        {
          text: "Videos",
          url: "#videos",
        },
        {
          text: "Fans",
          url: "#fans",
        },
        {
          text: "News",
          url: "#news",
        },
        {
          text: "Shop",
          url: "#shop",
        },
      ],
    };
  },
  mounted() {},
};
</script>

<template>
  <header>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="my-logo-container my-3">
                        <img src="../assets/img/dc-logo.png" alt="">
                    </div>
                    <div class="my-menu-container">
                        <a v-for="link in menuLinks" :href="link.url" class="mx-3">{{ link.text }}</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </header>
</template>

<style scoped>
    .my-logo-container img{
        width: 80%;
    }

    a{
        text-decoration: none;
        color: black;
    }
</style>
