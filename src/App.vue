<script>
import AppHeader from "./components/AppHeader.vue";
import AppContent from "./components/AppContent.vue";
import AppLinks from "./components/AppLinks.vue";
import AppFooter from "./components/AppFooter.vue";
import comics from "./assets/data/comics.js";

export default {
  components: { AppHeader, AppContent, AppLinks, AppFooter },
  data() {
    return { comics };
  },
};
</script>

<template>
  <AppHeader />
  <main>
    <AppContent :comicsList="comics" />
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
img {
  max-width: 100%;
}
</style>
