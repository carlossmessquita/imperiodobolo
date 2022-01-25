<template>
    <div class="container">
        <img alt="Logo Imperio do Bolo" src="../assets/logo.png" width="180" >
    </div>

    <Navbar />  
</template>

<script>
import Navbar from './Navbar.vue'
export default {
    name: 'Header',
    components: {
        Navbar
    },
}
</script>
<style scoped>
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        background: rgb(151, 85, 10);
    }

    img {
        margin-bottom: 1%;
        padding: 5px;
    }
</style>