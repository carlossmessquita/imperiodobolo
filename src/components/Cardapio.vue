<template>
    <div class="container">
        <iframe class="cardapio" src="https://drive.google.com/file/d/1kiPmW8zk-30FN-UNkLcijZTM0KcIOlvg/preview" width="350" height="480" allow="autoplay"></iframe>
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
        flex-direction: column;
        align-items: center;
        margin-top: 1%;
        margin-bottom: 1%;
    }
    @media only screen and (max-width: 600px) {
        .container {
            width: 250;
            height: 380;
        }
    }
</style>