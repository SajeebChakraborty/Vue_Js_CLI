<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h3>{{ title }}</h3>
  <Header></Header>

  <AllFriends :friends="friends"></AllFriends>
</template>

<script>
import Header from './components/Header.vue'
import AllFriends from './components/AllFriends.vue'

export default {
  name: 'App',
  data () {
    return {
      title: 'Welcome to Your Vue.js App',
      friends: [

                {name:"a",online:true},
                {name:"b",online:false},
                {name:"c",online:true},
                {name:"d",online:true},

        ]

    }
  },
  components: {
    Header,
    AllFriends,
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
