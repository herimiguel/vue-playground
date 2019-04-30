<template>
  <div id="Myapp">

    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  // name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
html{
  background-color: black;
  display: block;
}
#Myapp {
background-color: rgba(7, 1, 1, 0.947);
height: 100%;
width: 100%;
}
</style>
