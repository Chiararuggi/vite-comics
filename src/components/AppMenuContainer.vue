<script>
export default {
  name: "AppMenuContainer",
  data() {
    return {
      menuLinksComics: [
        {
          url: "Characters",
        },
        {
          url: "Comics",
        },
        {
          url: "Movies",
        },
        {
          url: "Tv",
        },
        {
          url: "Games",
        },
        {
          url: "Videos",
        },
        {
          url: "News",
        },
      ],
      menuLinksShop: [
        {
          url: "Shop DC",
        },
        {
          url: "Shop DC Collectibles",
        },
      ],
      menuLinksDC: [
        {
          url: "Terms Of USe",
        },
        {
          url: "Privacy policy(New)",
        },
        {
          url: "Ad choices",
        },
        {
          url: "Advertising",
        },
        {
          url: "Jobs",
        },
        {
          url: "Subscriptions",
        },
        {
          url: "Talent Workshops",
        },
        {
          url: "CPSC Certificates",
        },
        {
          url: "Ratings",
        },
        {
          url: "Shop Help",
        },
        {
          url: "Contact Us",
        },
      ],
      menuLinksSites: [
        {
          url: "DC",
        },
        {
          url: "Mad Magazine",
        },
        {
          url: "DC Kids",
        },
        {
          url: "DC Universe",
        },
        {
          url: "DC Power Visa",
        },
      ],
    };
  },
  mounted() {},
};
</script>

<template>
  <div class="my-container">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="my-menu-container d-flex justify-content-between">
            <div class="d-flex">
              <div class="d-flex flex-column my-5 my-mr3">
                <ul class="my-2">
                  DC COMICS
                </ul>
                <li v-for="link in menuLinksComics" class="my-mt1">
                  {{ link.url }}
                </li>
                <ul class="my-2">
                  SHOP
                </ul>
                <li v-for="link in menuLinksShop" class="my-mt1">
                  {{ link.url }}
                </li>
              </div>
              <div class="d-flex flex-column my-5 my-mr3">
                <ul class="my-2">
                  DC
                </ul>
                <li v-for="link in menuLinksDC" class="my-mt1">
                  {{ link.url }}
                </li>
              </div>
              <div class="d-flex flex-column my-5 my-mr3">
                <ul class="my-2">
                  SITES
                </ul>
                <li v-for="link in menuLinksSites" class="my-mt1">
                  {{ link.url }}
                </li>
              </div>
            </div>
            <div class="d-flex">
              <img src="/img/dc-logo-bg.png" class="logo-img" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.my-container {
  background-image: url("/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.my-menu-container{
    height:28rem;
}

ul {
  color: white;
  margin: 0;
  padding: 0;
}

li {
  color: #8f9288;
  list-style-type: none;
}

.my-mr3 {
  margin-right: 3rem;
}

.my-mt1 {
  margin-top: 0.1rem;
}

.logo-img{
    object-fit: cover;
    width: 40rem;
}
</style>
