//app.vue looks for a template, script, style

<template>
  <div id="app1">
    <img src="./assets/logo.png">
    <HelloWorld msg="Beth loves bootcamp!"/>

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld

  }
}

</script>

<style>
#app1 {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
