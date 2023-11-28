<script>
export default {
  name: "AppBlueContainer",
  data() {
    return {
      menuLinks: [
        {
          text: "DIGITAL COMICS",
          src: "../assets/img/buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          src: "../assets/img/buy-comics-mechandise.png",
        },
        {
          text: "SUBSCRIPTION",
          src: "../assets/img/buy-comics-subscriptions.png",
        },
        {
          text: "COMIC SHOP LOCATOR",
          src: "../assets/img/buy-comics-shop-locator.png",
        },
        {
          text: "DC POWER VISA",
          src: "../assets/img/buy-dc-power-visa.svg",
        },
      ],
    };
  },
  mounted() {},
};
</script>

<template>
  <div class="my-blue-container">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="d-flex justify-content-around">
            <div class="merch-card d-flex" v-for="card in menuLinks">
              <img :src="card.src" />
              <p>{{ card.text }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.my-blue-container {
  background-color: blue;
  color: white;
}
</style>
