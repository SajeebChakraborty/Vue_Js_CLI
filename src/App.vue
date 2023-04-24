<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h3>{{ title }}</h3>
  <Header></Header>
  <Hook ></Hook>
  <Post></Post>

  <AllFriends :friends="friends" @delete="deletefriend"></AllFriends>
</template>

<script>
import Header from './components/Header.vue'
import AllFriends from './components/AllFriends.vue'
import Hook from './components/Hook.vue'
import Post from './components/Post.vue'

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
  methods:{

    deletefriend(payload){

        this.friends = this.friends.filter(friend => friend.name !== payload.name)

    }

  },
  components: {
    Header,
    AllFriends,
    Hook,
    Post,
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
