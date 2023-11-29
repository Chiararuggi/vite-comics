<script>
export default {
  name: "AppFooter",
  data() {
    return {
      menuSocialLinks: [
        {
          src: "/img/footer-facebook.png",
        },
        {
          src: "/img/footer-twitter.png",
        },
        {
          src: "/img/footer-youtube.png",
        },
        {
          src: "/img/footer-pinterest.png",
        },
        {
          src: "/img/footer-periscope.png",
        },
      ],
    };
  },
  mounted() {},
};</script>

<template>
  <div class="my-container">
    <div class="container">
        <div class="row">
            <div class="col-12">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="my-button my-4">
                        <button class="my-btn">SIGN-UP NOW!</button>
                    </div>
                    <div class="my-social-container d-flex my-4">
                        <h6>FOLLOW US</h6>
                        <img v-for="img in menuSocialLinks" :src="img.src" class="mx-1">
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<style scoped>
.my-container {
  background-color: #303030;
}
.my-btn{
    color:white;
    border: 2px solid #047cec;
    padding: 0.5rem;
    background-color: transparent;
}

h6{
    color: #047cec;
    padding:0;
    margin: 0;
    align-self:center;
    margin-right: 1rem;
}
</style>
