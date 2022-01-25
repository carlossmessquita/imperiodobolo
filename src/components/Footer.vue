<template>
    <div class="footer">
        <p>
            Império do Bolo&#174; LTDA, Rua Pedro I, Centro, Fortaleza - Ce,
            CNPJ: {{ cnpj }}
        </p>
        <a href="https://carlos-mesquita.herokuapp.com">Desenvolvido por Carlos Mesquita</a>

    </div>
</template>
<script>

export default {
    name: 'Footer',
    data() {
        return {
            cnpj: '30.183.953/0001-01 '
        }
    }
}
</script>
<style scoped>
    .footer {
        display: flex;
        flex-direction: column;
        align-items: center;
        background: rgb(151, 85, 10);
        color: rgb(255, 200, 133);
        font-family: monospace;
        border-top: 1px solid rgb(255, 200, 133);
        padding: 15px;
        
    }
    a {
        text-decoration: none;
        font-family: monospace;
        color: rgb(59, 32, 0);
        margin-top: 3%;
    }
</style>