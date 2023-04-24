<template>

    <div class="Hook">

      
    </div>
    
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Hook',
    data () {
        return {
            
          

        }
    },
    beforeCreate() {
        console.log('beforeCreate')
    },
    created() {
        console.log('created')
    },
    beforeMount() {
        console.log('beforeMount')
    },
    mounted() {
        console.log('mounted')
    },
    beforeUpdate() {
        console.log('beforeUpdate')
    },
    updated() {
        console.log('updated')
    },

    methods: {
      


    }


}
</script>
<style scoped>

   

</style>