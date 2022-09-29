<template>
  <div id="app" class="one" img-src="https://samczsun.com/content/images/size/w2000/2020/09/109768371_xl.jpg">
    <HeaderOne />

    <CardsOne />

    <div class="text-center">
      <video id="video" controls muted autoplay name>
        <source src="./assets/video.mp4" type="video/mp4">
      </video>
    </div>

    <FooterOne />

  </div>
</template>

<script>
import HeaderOne from "./components/Header.vue";
import CardsOne from "./components/Cards.vue";
import FooterOne from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    HeaderOne,
    CardsOne,
    FooterOne,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Life+Savers:wght@700&display=swap');

#app {
  font-family: 'Life Savers', cursive;
  color: #2c3e50;
}

.one {
  background-image: linear-gradient(to bottom,
      rgba(10, 10, 10, 0.8),
      rgba(255, 99, 71, 0.5)),
    url("https://samczsun.com/content/images/size/w2000/2020/09/109768371_xl.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-attachment: fixed;
  background-size: auto;
}
</style>
