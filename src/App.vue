<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h3>{{ title }}</h3>
  <Header></Header>

        <nav>
            <ul>
                <li>Home</li>
                <li>Products</li>
                <li>Cart</li>
            </ul>
        </nav>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  data () {
    return {
      title: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    Header
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
