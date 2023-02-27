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
      <div class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo" />
        <ul>
          <li v-for="(link, index) in headerlinks" :key="index">
            <a :href="link.link">{{ link.text }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<style scoped lang="scss">
header {
  height: 200px;
  background-color: black;
  display: flex;
  nav {
    background-color: white;
    height: 70%;
    margin-top: auto;
    width: 100%;
    .container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      ul {
        list-style: none;
        display: flex;
        align-items: center;
        li {
          display: inline-block;
          margin-right: 1.5rem;
          text-transform: uppercase;
          border-bottom: 5px solid transparent;
          &:hover {
            border-bottom: 5px solid #0c7cec;
          }
          a {
            text-decoration: none;
            color: #333;
            font-weight: bold;
            font-size: 0.8rem;
            line-height: 100px;
            display: inline-block;
            &:hover {
              color: #0c7cec;
            }
          }
        }
      }
    }
    img {
      max-height: 70px;
    }
  }
}
</style>
