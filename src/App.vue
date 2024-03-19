<template>
  <main-header></main-header>
  <project-list></project-list>
  <carousel></carousel>
</template>

<script>
import mainHeader from './assets/UI/header.vue'
import projectList from './components/projects.vue'
import carousel from "@/assets/UI/carousel.vue";
export default {
  name: 'App',
  components: {
    mainHeader,
    projectList,
    carousel
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
