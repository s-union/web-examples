<script setup lang="ts">
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';
import Main from './components/Main.vue';
</script>

<template>
  <Header />
  <Main />
  <Footer />
</template>

<style>
body {
  font-size: 16px;
  width: 90%;
  max-width: 960px;
  margin-inline: auto;
  padding-inline: 8px;
}
</style>
