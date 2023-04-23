<template>

    <div class="Header">

        <nav>
            <ul>
                <li>Home</li>
                <li>Products</li>
                <li>Cart</li>
            </ul>
        </nav>

    </div>
    
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Header',
    data () {
        return {
            
        }
    }
}
</script>
<style scoped>

    .Header {
        background-color: #f1f1f1;
        padding: 20px;
    }

    nav {
        display: flex;
        justify-content: space-between;
    }

    ul {
        display: flex;
        list-style: none;
    }

    li {
        padding: 0 10px;
    }

</style>