<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Menu from './components/Menu.vue';
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
      <div class="content">
        <img alt="logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />
        <div class="greetings">
        <h1 class="green my-3">My name is Rendy Afriatama</h1>
        <h3>
            Backend Developer
        </h3>
      </div>
  </div>
   
    <RouterView />
    </div>
</template>

<style scoped>

.content{
  
  display: flex;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
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
