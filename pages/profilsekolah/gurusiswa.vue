<template>
  <div class="container mx-auto">
      <div class="grid grid-cols-2 mt-10 h-[100vh]">
          <v-card class="mx-auto text-center" min-width="500px" max-height="100px" title="Jumlah Siswa">
              <v-card-subtitle>
                  <p class="text-[20px] font-semibold">{{ data.siswa }}</p>
              </v-card-subtitle>
          </v-card>
          <v-card class="mx-auto text-center" min-width="500px" max-height="100px" title="Jumlah Rombel">
              <v-card-subtitle>
                  <p class="text-[20px] font-semibold">{{ data.rombel }}</p>
              </v-card-subtitle>
          </v-card>
          <v-card class="mx-auto text-center" min-width="500px" max-height="100px" title="Jumlah Guru">
              <v-card-subtitle>
                  <p class="text-[20px] font-semibold">{{ data.guru }}</p>
              </v-card-subtitle>
          </v-card>
          <v-card class="mx-auto text-center" min-width="500px" max-height="100px" title="Jumlah Tenaga Adinistrasi">
              <v-card-subtitle>
                  <p class="text-[20px] font-semibold">{{ data.administrasi }}</p>
              </v-card-subtitle>
          </v-card>
      </div>
  </div>
</template>

<script>
export default {
  data() {
      return {
          data: {
              siswa: "1116",
              rombel: "34",
              guru: "60",
              administrasi: "10",
          }
      };
  }
};
</script>

<style scoped></style>