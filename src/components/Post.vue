<template>

    <div class="Post">

        <input type="text" v-model="search" placeholder="Search" class="form-control">
        <div v-for="(post,index) in searchPost" :key="index">

            <span>{{post.title}}</span>

        </div>
      
    </div>
    
</template>

<script>
import axios from 'axios'


export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Post',
    data () {
        return {
            
          post:{},
          search:'',

        }
    },
    computed: {
        searchPost(){
            return this.post.filter((post) => {
                return post.title.match(this.search)
            })
        }
    },
    created(){

        axios.get('https://jsonplaceholder.typicode.com/posts')
        .then(response => {
            
            this.post = response.data

        })
        .catch(error => {
            console.log(error)
        })

    },
    methods: {
      


    }


}
</script>
<style scoped>

   

</style>