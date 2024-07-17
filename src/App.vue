<script setup>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppLogo from './components/AppLogo.vue';
import SearchContainer from './components/SearchContainer.vue';
</script>

<template>
  <AppHeader />

  <AppLogo />
  <SearchContainer />
  <div class="flex-grow" />

  <AppFooter />
</template>

<style scoped></style>
