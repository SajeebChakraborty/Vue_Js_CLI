<template>

    <div class="AllFriends">

        <div v-for="(friend,index) in friends" :key="index">

            <span>{{friend.name}}</span>

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
    }
}
</script>
<style scoped>

   

</style>