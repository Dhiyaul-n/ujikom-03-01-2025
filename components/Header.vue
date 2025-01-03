<template>
  <div class="header z-20 w-screen flex justify-center items-center p-6">
      <div>
          <img class="flex justify-start max-w-[200px]" src="../assets/img/header.png" alt="">
      </div>


      <div class="nav text-[18px]">
          <ul>
              <li>
                  <NuxtLink to="/">Beranda</NuxtLink>
              </li>
              <li>
                  <NuxtLink to="../artikel">Artikel</NuxtLink>
              </li>
              <li>
                  <a class="w-full" href="#">Profil Sekolah</a>
                  <ul>
                      <li>
                          <NuxtLink to="/profilsekolah/sejarah">Sejarah</NuxtLink>
                      </li>
                      <li>
                          <NuxtLink to="/profilsekolah/profil">Profil Sekolah</NuxtLink>
                      </li>
                      <li>
                          <NuxtLink to="/profilsekolah/gurusiswa">Data guru & siswa</NuxtLink>
                      </li>
                  </ul>
              </li>
              <li>
                  <NuxtLink to="../galery">Galeri</NuxtLink>
              </li>
              <li>
                  <NuxtLink to="../ekstrakulikuler">Ekstrakulikuler</NuxtLink>
              </li>
          </ul>
      </div>
  </div>

</template>


<style scoped>
.header {
  background: linear-gradient(180deg, #011a3b, #033d8c);
}

.nav {
  border-radius: 6px;
}

.nav ul {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

.nav ul li {
  list-style: none;
  padding: 5 px;
  position: relative;
  transition: 500ms;
  display: block;
}

.nav ul li a {
  color: white;
  text-decoration: none;
  padding: 5px 5px;
}

.nav ul li a:hover {
  color: #ffad00;
  border-radius: 6px;
  transition: ease-in-out 600ms;
}

.nav ul li ul {
  display: none;
}

.nav ul li:hover ul {
  display: block;
  position: absolute;
  background: linear-gradient(180deg, #011a3b, #033d8c);
  border-radius: 6px;
  width: max-content;
  z-index: 10;
}

.nav ul li ul a {
  color: white;
  padding-left: 10px;
  margin: 0;
}

.nav ul li ul a:hover {
  color: #ffad00;
}
</style>