<template>
  <div class="container mx-auto my-20">
      <div class="grid grid-cols-5 gap-10">
          <div v-for="(galery, i) in galery" :key="i" class=" bg-[#eee] rounded-xl hover:shadow-2xl ease-in-out grayscale hover:grayscale-0 scale-75 hover:scale-105 duration-500">
              <img class="rounded-2xl blur-sm hover:blur-0 duration-500 m-0 w-full" :src="`/img/galery/${galery.src}`">
              <div class="text text-center text-[15 px] font-playfair ">
                  <h1 class="text-center align-bottom p-2">{{ galery.name }}</h1>
              </div>
            </div>
      </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const galery = ref([
  { 
      name: "MPLS 2024",
      src: 'galery.jpg',
  },

  { 
      name: "Hari Guru 2024",
      src: 'galery1.jpg',
  },

  { 
      name: "Classmeet 2024",
      src: 'galery2.jpg',
  },

  { 
      name: "Upacara Kemerdekaan 2024",
      src: 'galery3.jpg',
  },

      { 
      name: "P5 Melamar Kerja",
      src: 'galery4.jpg',
  },
])
</script>

<style lang="scss" scoped>

</style>