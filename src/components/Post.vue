<template>

    <div class="Post">

        <div v-for="(post,index) in post" :key="index">

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
            
          post:{}

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