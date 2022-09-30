<template>
  <div id="app" img-src="https://samczsun.com/content/images/size/w2000/2020/09/109768371_xl.jpg">
    <HeaderOne />
    <video autoplay muted loop id="myVideo">
      <source src="./assets/lol.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <div class="header2 d-flex align-items-center justify-content-center mb-5" style="height: 100vh">
      <h1 data-text="WAR OF THE LEGENDS"><span>WAR OF THE LEGENDS</span></h1>
    </div>
    <CardsOne />
    <div class="text-center">
      <video id="video" controls muted autoplay name>
        <source src="./assets/video.mp4" type="video/mp4">
        <audio src="path/to/song.mp3" controls autoplay></audio>
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

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Life+Savers:wght@700&display=swap');

#app {
  font-family: 'Life Savers', cursive;
  color: #2c3e50;
  background-image: linear-gradient(to bottom,
      rgba(10, 10, 10, 0.8),
      rgba(255, 99, 71, 0.5)),
    url("https://samczsun.com/content/images/size/w2000/2020/09/109768371_xl.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-attachment: fixed;
  background-size: auto;
  animation: fade-in 1.5s ease, slide-in 1.2s ease;
  scroll-behavior: smooth;
}

//Animations
@keyframes fade-in {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes slide-in {
  0% {
    top: -300px;
  }

  100% {
    top: 0;
  }
}

h1 {
  position: relative;
  font-size: 80px;
  font-size: calc(10px + 5vw);
  color: #fff;
  letter-spacing: 0.02em;
  text-transform: uppercase;
  text-shadow: 0 0 0.15em #1da9cc;
  white-space: nowrap;
  filter: blur(0.007em);
  animation: shake 2.5s;
}

h1 span {
  position: absolute;
  transform: translate(-50%, -50%);
  -webkit-clip-path: polygon(10% 0%, 44% 0%, 70% 100%, 55% 100%);
  clip-path: polygon(10% 0%, 44% 0%, 70% 100%, 55% 100%);
}

h1::before,
h1::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  // left: 0;
}

h1::before {
  animation: crack1 2.5s linear forwards;
  -webkit-clip-path: polygon(0% 0%, 10% 0%, 55% 100%, 0% 100%);
  clip-path: polygon(0% 0%, 10% 0%, 55% 100%, 0% 100%);
}

h1::after {
  animation: crack2 2.5s linear forwards;
  -webkit-clip-path: polygon(44% 0%, 100% 0%, 100% 100%, 70% 100%);
  clip-path: polygon(44% 0%, 100% 0%, 100% 100%, 70% 100%);
}

@keyframes shake {

  5%,
  15%,
  25%,
  35%,
  55%,
  65%,
  75%,
  95% {
    filter: blur(0.018em);
    transform: translateY(0.018em) rotate(0deg);
  }

  10%,
  30%,
  40%,
  50%,
  70%,
  80%,
  90% {
    filter: blur(0.01em);
    transform: translateY(-0.018em) rotate(0deg);
  }

  20%,
  60% {
    filter: blur(0.03em);
    transform: translate(-0.018em, 0.018em) rotate(0deg);
  }

  45%,
  85% {
    filter: blur(0.03em);
    transform: translate(0.018em, -0.018em) rotate(0deg);
  }

  100% {
    filter: blur(0.007em);
    transform: translate(0) rotate(-0.5deg);
  }
}

@keyframes crack1 {

  0%,
  95% {
    transform: translate(-50%, -50%);
  }

  100% {
    transform: translate(-51%, -48%);
  }
}

@keyframes crack2 {

  0%,
  95% {
    transform: translate(-50%, -50%);
  }

  100% {
    transform: translate(-49%, -53%);
  }
}

.header2 {
  background: black;
  // font-family: 'Montserrat', Arial, sans-serif;
}

#myVideo {
  position: absolute;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0.8;
}

#video {
  width: 100%;
}
</style>
