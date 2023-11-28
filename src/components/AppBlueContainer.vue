<script>
export default {
  name: "AppBlueContainer",
  data() {
    return {
      menuLinks: [
        {
          text: "DIGITAL COMICS",
          src: "/img/buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          src: "/img/buy-comics-merchandise.png",
        },
        {
          text: "SUBSCRIPTION",
          src: "/img/buy-comics-subscriptions.png",
        },
        {
          text: "COMIC SHOP LOCATOR",
          src: "/img/buy-comics-shop-locator.png",
        },
        {
          text: "DC POWER VISA",
          src: "/img/buy-dc-power-visa.svg",
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
          <div class="my-card d-flex justify-content-around align-items-center">
            <div class="merch-card d-flex" v-for="card in menuLinks">
              <img :src="card.src" class="card-img"/>
              <p class="card-text">{{ card.text }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.my-blue-container {
  background-color: #0282f9;
  color: white;
}

.my-card img{
    width: 3rem;
    margin-top: 2rem;
    margin-bottom: 2rem;
}

.card-text{
    align-self: center;
    margin-right: 2rem;
    margin-left: 2rem;
    font-size: 0.7rem;
}
</style>
