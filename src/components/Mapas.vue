<template>
    <div class="botao">
        <h3>Com sabor, com amor, pra você!</h3>
        <button @click="verMapas">Ver Localização</button>
    </div>
    
    <div v-show="mostrar_mapa" class="mapas">
        <p>Rua Pedro I, 931, Centro, Fortaleza - Ce 
        <br> 
        Telefone: {{ telefone_um }}</p>  
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15925.246918949224!2d-38.54092965223696!3d-3.7421055128786183!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x7c749aead41ac7d%3A0xc0d130c863255a99!2sImperio%20do%20Bolo!5e0!3m2!1spt-BR!2sbr!4v1643145320006!5m2!1spt-BR!2sbr" width="300" height="200" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        <p>Rua Floriano Peixoto, 748, Centro, Fortaleza - Ce
        <br> 
        Telefone: {{ telefone_dois }}</p> 
        <iframe class="mapa" src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d7962.742701207058!2d-38.527749!3d-3.7289640000000004!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x5141b12cb21eb557!2sImp%C3%A9rio%20do%20bolo!5e0!3m2!1spt-BR!2sbr!4v1640101385163!5m2!1spt-BR!2sbr" width="300" height="200" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    </div>
</template>
<script>
export default {
    name: 'Mapas',
    data() {
        return {
            telefone_um: '(85) 3045-4549',
            telefone_dois: '(85) 3253-2562',
            mostrar_mapa: false
        }
    },
    methods: {
        verMapas() {
            this.mostrar_mapa = !this.mostrar_mapa;
        }
    }
}
</script>
<style scoped>
    .mapas {
        display: flex;
        justify-content: space-evenly;
        padding: 25px;
        background: rgba(151, 85, 10, 0.781);
        align-items: center;
    }

    .botao {
        display: flex;
        flex-direction: column;
        align-items: center;
        background: rgb(151, 85, 10);
        color: rgb(255, 200, 133);
        font-family: monospace;
        border-top: 1px solid rgb(255, 200, 133);
        padding: 15px;
    }

    button {
        margin-top: 2%;
        padding: 10px;
        border: none;
        border-radius: 5px;
        color: rgb(151, 85, 10);
        font-weight: bold;
        background: rgb(255, 210, 156);
        cursor: pointer;
    }

    h3 {
        font-weight: bold;
        font-size: 18px;
    }
    p {
        background: rgb(255, 200, 133);
        padding: 5px;
        color: rgb(151, 85, 10);
        font-family: monospace;
    }

    iframe {
        margin-bottom: 3%;
    }


    @media only screen and (max-width: 600px) {
        .mapas {
            flex-direction: column;
            align-items: center;
        }
    }
</style>