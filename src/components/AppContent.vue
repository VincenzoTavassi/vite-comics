<script>
import AppCard from "./AppCard.vue";
export default {
  components: { AppCard },
  props: { comicsList: Array },
  data() {
    return {};
  },
};
</script>

<template>
  <section>
    <div class="jumbotron"></div>
    <div class="container">
      <div id="current-series">CURRENT SERIES</div>
      <AppCard
        v-for="comic in comicsList"
        :title="comic.series"
        :image="comic.thumb"
      />
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/mixins.scss" as *;

section {
  background-color: black;
  color: white;
  font-size: 2rem;
  font-weight: bold;
  .jumbotron {
    background-image: url("../assets/img/jumbotron.jpg");
    height: 45vh;
  }
  .container {
    max-width: 1200px;
    margin: 0 auto;
    position: relative;
    padding: 50px 0;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    #current-series {
      background-color: $brand-blue;
      color: white;
      padding: 15px 30px;
      display: inline-block;
      font-size: 1.3rem;
      position: absolute;
      top: 0;
      left: 0;
      transform: translate(0, -50%);
    }
  }
}
</style>
