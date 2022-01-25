<template>
    <Header />
    <Cardapio />
    <Mapas />
    <Footer /> 
</template>

<script>
import Header from './components/Header.vue'
import Cardapio from './components/Cardapio.vue'
import Mapas from './components/Mapas.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
      Header,
      Cardapio,
      Mapas,
      Footer
  }
}
</script>

<style>
    body {
        background: #FFEFBA;  /* fallback for old browsers */
        background: -webkit-linear-gradient(to left, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
        background: linear-gradient(to left, #FFFFFF, #FFEFBA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    }

</style>
