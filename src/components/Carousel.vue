<template>
    <div class="q-pa-md">
      <q-carousel
        animated
        v-model="slide"
        arrows
        navigation
        infinite
      >
          <q-carousel-slide :name="1" img-src="src/assets/IMG-20240526-WA0019.jpg" class="carousel-img" />
          <q-carousel-slide :name="2" img-src="https://down-id.img.susercontent.com/file/sg-11134201-22120-rohabay0oplv05" class="carousel-img" />
          <q-carousel-slide :name="3" img-src="https://down-id.img.susercontent.com/file/sg-11134201-22120-y52btabtpplv95"class="carousel-img" />
          <q-carousel-slide :name="4" img-src="https://down-id.img.susercontent.com/file/id-11134207-7qukw-lhxmo4v9a67e02" class="carousel-img" />
      </q-carousel>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue'
  
  export default {
    setup () {
      return {
        slide: ref(1)
      }
    }
  }
  </script>
  
  <style scoped>
  .carousel-img {
    width: 100%; /* Menggunakan lebar 100% agar gambar terlihat responsif */
    height: 1080px; /* Menggunakan ketinggian otomatis agar gambar tetap proporsional */
    max-height: 100px; /* Atur ketinggian maksimum agar gambar tidak terlalu besar */
    background-size: contain; /* Menggunakan contain untuk memastikan gambar tetap proporsional */
    background-position: center; /* Posisikan gambar di tengah-tengah */
  }
  </style>
  