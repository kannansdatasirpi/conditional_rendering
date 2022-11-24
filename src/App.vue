<template>
  
  <conditional_rendering />
</template>

<script>
import conditional_rendering from './components/conditional_rendering.vue'

export default {
  name: 'App',
  components: {
    conditional_rendering
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
