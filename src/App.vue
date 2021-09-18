<template>
  <div id="app">
    <div class="container">
        <div class="row">
            <Nav />
        </div>

        <div class="row">
            <img alt="Vue logo" src="./assets/logo.png" style="max-width: 100px;">
        </div>

        <div class="row">
            <Demo />
        </div>
    </div>
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Demo from './components/Demo.vue'

export default {
  name: 'App',
  components: {
    Nav,
    Demo
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
