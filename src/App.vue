<template>
  <main-header></main-header>
  <project-list></project-list>
  <carousel></carousel>
  <about-us></about-us>
  <main-order></main-order>
  <main-footer></main-footer>
</template>

<script>
import mainHeader from './assets/UI/header.vue'
import projectList from './components/projects.vue'
import carousel from "@/assets/UI/carousel.vue";
import aboutUs from './assets/UI/aboutUs.vue'
import mainOrder from './assets/UI/order.vue'
import mainFooter from './assets/UI/footer.vue'
// import mainInput from "@/components/projects";
export default {
  name: 'App',
  components: {
    mainHeader,
    projectList,
    carousel,
    aboutUs,
    mainOrder,
    mainFooter
  }
}
</script>

<style>
/*@font-face {*/
/*  font-family: Lucida;*/
/*  src: url("");*/
/*}*/

body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /*margin-top: 60px;*/
  box-sizing: border-box;
}

body::-webkit-scrollbar {
  width: 5px;
}

body::-webkit-scrollbar-track {
  background-color: transparent;
  background-image: linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));
}

body::-webkit-scrollbar-thumb {
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
}


.container {
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
}

.container {
  padding-top: 155px;
  padding-bottom: 115px;
}

.purple {
  background-image: linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));
}

.title {
  position: absolute;
  top: 75px;
  left: -100px;
  text-transform: uppercase;
  font-size: 120px;
  margin: 0;
  z-index: 1;
}

.title.linear {
  color: transparent;

  background-image: linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.title.white {
  color: rgba(255, 255, 255, 0.5);
}

.container.header, .container.footer {
  padding: 25px 13px;
}

.btn {
  padding: 15px 25px;
  border-radius: 8px;
  border: none;
  color: white;
  background-image: linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));
}


</style>
