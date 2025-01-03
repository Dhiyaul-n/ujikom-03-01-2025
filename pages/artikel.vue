<template>
  <div class="wrapper w-screen">
    <div class="container mx-auto my-20">
      <div class="grid grid-cols-2 gap-14">
        <div v-for="(artikel, i) in artikel" :key="i"
          class="bg-[#eee] hover:shadow-2xl ease-in-out duration-700  w-[100%] flex h-full rounded-lg" :height="200" rounded>
          <img class="h-[100px]" :src="`/img/news/${artikel.src}`">
          <div class="">
            <a href="" class="text-[20px] font-sans text-blue-500">{{ artikel.name }}</a>
            <p class="date">{{ artikel.date }}</p>
            <p class="penerbit">{{ artikel.penulis }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>


const artikel = ref([
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },

  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "03-01-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },

])
</script>

<style lang="scss" scoped></style>
