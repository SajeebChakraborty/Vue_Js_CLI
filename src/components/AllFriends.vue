<template>

    <div class="AllFriends">

        <div v-for="(friend,index) in friends" :key="index">

            <span>{{friend.name}}</span>
            <button @click="unfriend(friend.name)">Unfriend</button>

        </div>

    </div>
    
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'AllFriends',
    props: ['friends'],
    data () {
        return {
            
          

        }
    },
    methods: {
        unfriend(name) {
            this.$emit('delete', { name })
        }
  }


}
</script>
<style scoped>

   

</style>