<template>
 <img src="./assets/logo.png" />
 <ComponentOne />
</template>

<script>
import ComponentOne from './components/ComponentOne.vue';

export default {
  name: 'App',
  components: {
   ComponentOne,
  },
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
