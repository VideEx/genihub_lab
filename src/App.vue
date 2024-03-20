<template>
  <main-header></main-header>
  <project-list></project-list>
  <carousel></carousel>
  <about-us></about-us>
  <main-order></main-order>
</template>

<script>
import mainHeader from './assets/UI/header.vue'
import projectList from './components/projects.vue'
import carousel from "@/assets/UI/carousel.vue";
import aboutUs from './assets/UI/aboutUs.vue'
import mainOrder from './assets/UI/order.vue'
// import mainInput from "@/components/projects";
export default {
  name: 'App',
  components: {
    mainHeader,
    projectList,
    carousel,
    aboutUs,
    mainOrder
  }
}
</script>

<style>
#app {
  margin: 0;
  padding: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /*margin-top: 60px;*/
}
</style>
