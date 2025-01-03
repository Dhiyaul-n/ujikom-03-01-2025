<template>
  <div class="container mx-auto h-[100%]">
      <div class=" justify-center border-2 m-10 p-10">

          <h1 class="text-center text-[40px] m-10 font-playfair">Identitas Sekolah Menengah Kejuruan Negeri 4 Tasikmalaya</h1>

          <div class="tabel container px-5">
              <table class=" border-2 p-10 my-10 w-full">
                  <tbody>
                      <tr>
                          <td>Nama Sekolah :</td>
                          <td>{{ data.name }}</td>
                      </tr>
                      <tr>
                          <td>NPSN :</td>
                          <td>20276063</td>
                      </tr>
                      <tr>
                          <td>Nomor Statistik Sekolah :</td>
                          <td>{{ data.npsn }}</td>
                      </tr>
                      <tr>
                          <td>Alamat :</td>
                          <td>{{ data.address }}</td>
                      </tr>
                      <tr>
                          <td>Website :</td>
                          <td>{{ data.website }}</td>
                      </tr>
                      <tr>
                          <td>E-mail :</td>
                          <td>{{ data.email }}</td>
                      </tr>
                      <tr>
                          <td>Nomor Statistik Sekolah :</td>
                          <td>{{ data.schoolStatNumber }}</td>
                      </tr>
                      <tr>
                          <td>Tahun Berdiri :</td>
                          <td>{{ data.foundingYear }}</td>
                      </tr>
                      <tr>
                          <td>Nomor SK Pendirian :</td>
                          <td>{{ data.establishmentSKNumber }}</td>
                      </tr>
                      <tr>
                          <td>Tanggal :</td>
                          <td>{{ data.establishmentDate }}</td>
                      </tr>
                  </tbody>
              </table>
          </div>
      </div>

  </div>
</template>

<script setup>

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

</script>

<style scoped>

tr, td, th {
  border: 2px solid #eee;
  padding: 10px;
}
</style>