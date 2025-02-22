<template>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>

body, html {
  margin: 0; /* Elimină marginile implicite */
  padding: 0; /* Elimină umplerea implicită */
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  /* background-color: #222021; */
  min-height: 100vh;
}
</style>
