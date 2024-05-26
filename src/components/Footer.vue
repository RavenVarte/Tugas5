<template>
    <q-footer class="bg-primary text-white q-pa-md">
      <div class="row items-center justify-between q-mb-md">
        <div class="col-auto">
          <q-avatar square size="56px">
            <img src="https://tse3.mm.bing.net/th?id=OIP.X9vvhHTBfcxhqE_y_e1A0AHaFB&pid=Api&P=0&h=180" alt="Logo">
          </q-avatar>
        </div>
        <div class="col-auto">
          <div class="text-h6">Ebby Farm</div>
          <div class="text-subtitle2">Jl. Aur Kuning , Pekanbaru</div>
          <div class="text-caption">Email: @EbbyFarm| Telepon: 0858-3612-2252</div>
        </div>

        </div>
      <div class="text-center q-pt-md">
        &copy; 2024 Toko Online Saya
      </div>
    </q-footer>
  </template>
  
  <script>
  export default {
    name: 'Footer',
    methods: {
      goTo(url) {
        window.open(url, '_blank')
      }
    }
  }
  </script>
  
  <style scoped>
  .q-footer {
    border-top: 1px solid rgba(255, 255, 255, 0.2);
    display: flex;
  }
  .row {
    display: flex;
    width: auto;
    height: auto;
  }
  </style>