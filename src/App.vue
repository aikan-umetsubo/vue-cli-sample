<template>
  <div id="app">
    <Top msg="This is top"/>
    <HelloWorld msg="And this is HelloWorld"/>
  </div>
</template>

<script>
import Top from './components/Top.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    Top,
    HelloWorld
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
