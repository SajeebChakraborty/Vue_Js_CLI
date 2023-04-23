<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h3>{{ title }}</h3>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      title: 'Welcome to Your Vue.js App'
    }
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
