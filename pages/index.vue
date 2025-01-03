<template>
  <div class="wrapper w-screen ">
    <div class="content mx-auto w-[100%] ">
            <v-carousel height="500" class="relative h-[80vh] w-[100%]">
                <v-carousel-item class="rounded-lg w-" v-for="(item, i) in items" :key="i" :src="`/img/carousel/${item.src}`"
                    reverse-transition="fade-transition" transition="fade-transition"></v-carousel-item>
            </v-carousel>
        </div>

    <div class="container mx-auto">
      <div class="flex justify-center p-20 container mx-auto">
        <div class="grid grid-cols-2 max-w-[1200px]">
          <div class="card flex justify-center">
            <div class=" rounded-[1rem] hover:shadow-2xl duration-500 ease-in-out p-6 bg-[#efefef] mr-5">
              <img src="../assets/img/kepala-sekolah.png" alt="Avatar" style="width:100%">
              <div class="container">
                <h2><b>KEPALA SEKOLAH</b></h2>
                <p></p> Kurniawan s.pd m.pd
              </div>
            </div>
          </div>
          <div class="rounded-[1rem] hover:shadow-2xl duration-500 ease-in-out">
            <p class="text-justify font-serif font-italic text-[14px] p-10">
              Assalamu'alaikum warahmatullahi wabarakatuh, Salam sejahtera, Shalom, Om Swastiastu, Namo
              Buddhaya Yang saya hormati, Para Wakil Kepala Sekolah, Guru, Staf, dan
              Siswa.<br><br>Alhamdulillah, kita dapat berkumpul dalam acara ini berkat rahmat Allah SWT.
              Terima kasih atas kehadiran semua pihak yang telah mendukung acara ini. Saya bangga dengan
              kerja keras dan kontribusi semua pihak dalam mendukung kemajuan sekolah kita. Pendidikan
              tidak hanya tentang ilmu, tetapi juga tentang pembentukan karakter. Untuk itu, mari kita
              terus bekerja sama agar sekolah ini terus maju dan memberikan pendidikan terbaik untuk masa
              depan yang gemilang. Semoga kita selalu diberikan kesehatan dan kekuatan untuk terus
              berusaha memberikan yang terbaik. Terima kasih atas perhatian dan kerjasamanya.
              Wassalamu'alaikum warahmatullahi wabarakatuh. Semoga rangkuman ini sesuai dengan yang Anda
              harapkan!
            </p>
          </div>
        </div>
      </div>

        <div class="text-center mt-28">
          <h1 class="text-[40px] py-10">Artikel Berita</h1>
        </div>

      <div class="grid grid-cols-2 gap-14 mb-28">
        <div v-for="(artikel, i) in artikel" :key="i"
          class="bg-[#eee] hover:shadow-2xl ease-in-out duration-700  w-[100%] flex h-full rounded-lg" :height="200"
          rounded>
          <img class="h-[100px]" :src="`/img/news/${artikel.src}`">
          <div class="">
            <a class="pl-5 text-[20px] font-serif text-blue-500">{{ artikel.name }}</a>
            <p class="pl-5 date">{{ artikel.date }}</p>
            <p class="pl-5 penerbit">{{ artikel.penulis }}</p>
          </div>
        </div>
      </div>


      <h1 class="text-center text-[40px] pt-32 pb-10">Jumlah Guru dan Siswa</h1>
      <div class="grid grid-cols-2 my-10">
        <v-card class="mx-auto text-center" min-width="500px" max-height="100px" title="Jumlah Siswa">
          <v-card-subtitle>
            <p class="text-[20px]">{{ Data.siswa }}</p>
          </v-card-subtitle>
        </v-card>

        <v-card class="mx-auto text-center mb-20" min-width="500px" max-height="100px" title="Jumlah Guru">
          <v-card-subtitle>
            <p class="text-[20px]">{{ Data.guru }}</p>
          </v-card-subtitle>
        </v-card>
      </div>

      <div class="flex justify-center">
        <iframe class="max-w-[1000px] p-20"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3957.213116362029!2d108.25189907500041!3d-7.329945292678408!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f59eeb6bda36f%3A0xa9e724a275da6c2d!2sSMK%20Negeri%204%20Tasikmalaya!5e0!3m2!1sid!2sid!4v1735548496522!5m2!1sid!2sid"
          width="100%" height="500px" style="" allowfullscreen="" loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    Data: {
      siswa: "1116",
      rombel: "34",
      guru: "60",
      administrasi: "10",
    }
  })
};
</script>

<style scoped>
.wrapper {
  background: white;
}

.content{
  background-color: #001550;
}

</style>

<script setup>


const artikel = ref([
  {
    name: "Pengumuman Ujikom",
    date: "02-02-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },

  {
    name: "Pengumuman Ujikom",
    date: "02-02-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "02-02-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
  {
    name: "Pengumuman Ujikom",
    date: "02-02-2025",
    penulis: "SMKN 4 TASIKMALAYA",
    src: 'news.1.jpg',
  },
])

const data = {
  name: "SMKN 4 Tasikmalaya",
  npsn: "20276063",
  schoolStatNumber: "401327810004",
  address: "Jl Depok RT 02 RW 05, Sukamenak, Purbaratu, Tasikmalaya, Jawa Barat",
  website: "www.smkn4-tsm.sch.id",
  email: "info@smkn4-tsm.sch.id",
  foundingYear: 2010,
  establishmentSKNumber: "420/9/SK-BPPT/2012",
  establishmentDate: "06 Februari 2012"
};

const items = ref([
    {
        src: 'homeimg.jpg',
    },
    {
        src: 'carousel.jpeg',
    },
    {
        src: 'profil.jpg',
    },
])

</script>