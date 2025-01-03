<template>
  <div class="container mx-auto flex justify-center items-center">
      <div class="grid grid-cols-5 gap-5 my-5">
          <v-sheet v-for="(ekskul, i) in ekskul" :key="i"
              class="flex bg-[#eee]  hover:shadow-2xl ease-in-out duration-700 rounded-xl px-5"
              :height="200" :width="200" rounded>
              <img class="rounded-2xl" :src="`/img/ekskul/${ekskul.src}`">
              <div class="text text-center font-bold text-[14px]">
                  <h1>{{ ekskul.name }}</h1>
              </div>
          </v-sheet>
      </div>
  </div>
</template>

<script setup>

const ekskul = ref([
  { src: 'basket.jpg', name: "Basket" },
  { src: 'bola.jpg', name: "Sepak Bola" },
  { src: 'bulutangkis.jpg', name: "Bulu Tangkis" },
  { src: 'cinema.jpg', name: "Cinemato Grafi" },
  { src: 'EC.jpg', name: "English Club" },
  { src: 'futsal.jpg', name: "Futsal" },
  { src: 'IRMA.jpg', name: "IRMA" },
  { src: 'ITClub.jpg', name: "IT Club" },
  { src: 'laskar.jpg', name: "Laskar Pustaka" },
  { src: 'OSIS.jpg', name: "OSIS" },
  { src: 'paskibra.jpg', name: "Paskibra" },
  { src: 'PD.jpg', name: "Perisai Diri" },
  { src: 'PKS.jpg', name: "PKS" },
  { src: 'PLH.jpg', name: "PLH" },
  { src: 'PMR.jpg', name: "PMR" },
  { src: 'pramuka.jpg', name: "Pramuka" },
  { src: 'PUB.jpg', name: "Pendidikan Untuk Bela Negara" },
  { src: 'safety.jpg', name: "Safety Riding" },
  { src: 'senitari.jpg', name: "Seni Tari" },
  { src: 'voly.jpg', name: "Voly" },
])

</script>

<style lang="scss" scoped></style>