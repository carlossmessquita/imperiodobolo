<template>
    <div class="container">
        <img src="img/valores.jpg" alt="" >           
        <img src="img/kitfestaib.png" alt="" width="375" height="475">
    </div>
    
</template>
<script>
export default {
    name: 'Cardapio',
}
</script>
<style scoped>
    .container {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        margin-top: 1%;
        margin-bottom: 1%;
    }

    img {
        width: 375px; 
        height: 475px;
    }
    @media only screen and (max-width: 600px) {
        .container {
            
            flex-direction: column;
            width: 250;
            height: 380;
        }

        img {
            margin-bottom: 25px;
            width: 250px;
            height: 375px;
        }
    }
</style>