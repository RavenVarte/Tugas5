<template>
  <q-layout>
    <Navbar />
    <q-page-container>
      <Carousel />
      
    </q-page-container>
    <Footer />
    
  </q-layout>
  
</template>

<script>
import Navbar from './components/Navbar.vue'
import Carousel from './components/Carousel.vue'
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    Footer
  }
}
</script>

<style>
/* Tambahkan styling global jika diperlukan */
</style>
