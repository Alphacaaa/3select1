<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/header.vue'



</script>

<template>
  <div class="header">
    <Header />
  </div>

  <div class="content">
    <RouterView />
  </div>
</template>

<style scoped>
.header{
  height: 100px;
  width: 100dvw;
}
</style>
