<script>
export default {
  data() {
    return {
      headerlinks: [
        { text: "characters", active: false, link: "#" },
        { text: "comics", active: false, link: "#" },
        { text: "movies", active: false, link: "#" },
        { text: "tv", active: false, link: "#" },
        { text: "collectibles", active: false, link: "#" },
        { text: "videos", active: false, link: "#" },
        { text: "fans", active: false, link: "#" },
        { text: "news", active: false, link: "#" },
        { text: "shop", active: false, link: "#" },
      ],
    };
  },
};
</script>

<template>
  <header>
    <nav>
      <img src="../assets/img/dc-logo.png" alt="Logo" />
      <ul>
        <li v-for="(link, index) in headerlinks" :key="index">
          <a :href="link.link">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  height: 200px;
  background-color: black;
  display: flex;
}

nav {
  background-color: white;
  height: 70%;
  margin-top: auto;
  width: 100%;
  display: flex;
  justify-content: space-between;
}
</style>
