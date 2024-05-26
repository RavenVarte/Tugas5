<template>
    <q-carousel
      animated
      v-model="slide"
      infinite
      navigation
      arrows
      :autoplay="2500"
    >
      <q-carousel-slide
        v-for="(image, index) in images"
        :name="index"
        :img-src="image.src"
        key="index"
      >
        <!-- Caption untuk setiap gambar -->
        <div class="caption">{{ image.caption }}</div>
      </q-carousel-slide>
    </q-carousel>
  </template>
  
  <script>
  export default {
    name: 'MyCarousel',
    data() {
      return {
        slide: 0,
        images: [
          {
            src: 'https://tse2.mm.bing.net/th?id=OIP.xKfRrS-tPssFSzC1wjnDpwHaEK&pid=Api&P=0&h=180',
            caption: 'Pisang'
          },
          {
            src: 'https://tse1.mm.bing.net/th?id=OIP.143mk3Og5ZMoOzzWyqfAOAHaEo&pid=Api&P=0&h=180',
            caption: 'Belimbing'
          },
          {
            src: 'https://tse4.mm.bing.net/th?id=OIP.5FcgbFmOyQDP_Sz143oGbgHaFj&pid=Api&P=0&h=180',
            caption: 'Semangka'
          },
          {
            src: 'https://tse2.mm.bing.net/th?id=OIP.ap8wjv3LDK_9FPXrH_p7GAHaHd&pid=Api&P=0&h=180',
            caption: 'Apel'
          },
          {
            src: 'https://tse4.mm.bing.net/th?id=OIP.D1STR9FD0GtuV7LigtjdvwHaEp&pid=Api&P=0&h=180',
            caption: 'Mangga'
          },
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .q-carousel {
    height: 700px;
    width: 1348px;
  }
  
  .q-carousel-slide {
    background-position: center;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .caption {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: #fff;
    padding: 10px;
    border-radius: 10px;
    font-size: 30px;
  }
  </style>