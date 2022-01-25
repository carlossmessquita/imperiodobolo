<template>
    <div class="links">
        <a v-for="link in links" v-bind:key="link.id" :href="link.link" target="_blank">{{ link.titulo }}</a>
    </div>

</template>
<script>
export default {
    name: 'Navbar',
    data() {
        return {
            links: [
                {id:1, link:"https://wa.me/5585999906418", titulo: 'Whatsapp'},
                {id:2, link:"https://www.ifood.com.br/delivery/fortaleza-ce/imperio-do-bolo-centro/92b7a7b6-1a78-4d7d-b22a-784c91c71911", titulo: 'Ifood'},
                {id:3, link:"https://www.instagram.com/imperiodobolo_ce/", titulo: 'Instagram'},
            ]
        }
    }
}
</script>
<style scoped>
    .links {
        display: flex;
        flex-direction: row;
        text-align: center;
        justify-content: space-evenly;
        border-bottom: 1px solid rgb(151, 85, 10);
    }
    a {
        padding: 10px;
        font-size: 15px;
        text-decoration: none;
        font-family: monospace;
        font-weight: bold;
        color: rgb(151, 85, 10);
        
    }
    a:hover {
        background: rgba(151, 85, 10, 0.185);
    }

    @media only screen and (max-width: 600px) {
        .links {
            flex-direction: column;
        }
    }
</style>