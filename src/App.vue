<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
  import 'bootstrap3/dist/css/bootstrap.min.css'
  import 'bootstrap3/dist/js/bootstrap.min'
  import HelloWorld from "./components/HelloWorld";
export default {
  name: 'App',
  components: {HelloWorld}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
