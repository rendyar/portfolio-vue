<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Menu from './components/Menu.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->
   
    <div class="container">
      <Menu />
      <div class="content my-5">
        <img alt="logo" class="logo mx-5" src="@/assets/foto.jpg" width="250" height="370" />
        <div class="greetings">
        <h1 class="green my-3">My name is Rendy Afriatama</h1>
        <h3>
            Backend Developer
        </h3>
        <p>
          Saya seorang anak muda berusia 17 tahun. saya bersekolah di SMK Taruna Bhakti Depok <br> dengan jurusan Rekayasa Perangkat Lunak. selain keseharian belajar membuat website <br>
           dan mendalami role backend, saya juga memiliki ketertarikan di dalam cyber security <br> terutama bagian kerentanan website sejak SMP
        </p>
      </div>
  </div>
   
    <RouterView />
    </div>
    <Footer />
</template>

<style scoped>

.content{
  
  display: flex;
}

p {
  margin-top: 60px;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.6rem;
  margin-top: 30px;
}

.name h1,
.name h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .name h1,
  .name h3 {
    text-align: left;
  }
}
</style>
