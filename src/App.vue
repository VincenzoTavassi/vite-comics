<script setup>
import AppHeader from "./components/AppHeader.vue";
import AppContent from "./components/AppContent.vue";
import AppLinks from "./components/AppLinks.vue";
import AppFooter from "./components/AppFooter.vue";
</script>

<template>
  <AppHeader />
  <main>
    <AppContent />
    <AppLinks />
  </main>
  <AppFooter />
</template>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
