<script>
export default {
  data() {
    return {
      headerlinks: [
        { text: "characters", active: false, link: "#" },
        { text: "comics", active: true, link: "#" },
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
          <li
            v-for="(link, index) in headerlinks"
            :key="index"
            :class="link.active ? 'active' : ''"
          >
            <a :href="link.link">{{ link.text }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<style scoped lang="scss">
@use "../assets/scss/mixins.scss" as *;
header {
  height: 150px;
  background-color: black;
  display: flex;
  nav {
    background-color: white;
    margin-top: auto;
    width: 100%;
    height: 75%;
    @include flex-center;
    align-items: flex-end;
    .container {
      width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      ul {
        list-style: none;
        li {
          display: inline-block;
          margin-right: 1.5rem;
          text-transform: uppercase;
          border-bottom: 5px solid transparent;
          &:hover {
            border-bottom: 5px solid $brand-blue;
          }
          &.active {
            border-bottom: 5px solid $brand-blue;
            color: #0c7cec;
          }
          a {
            text-decoration: none;
            color: inherit;
            font-weight: bold;
            font-size: 0.8rem;
            line-height: 80px;
            display: inline-block;
            &:hover {
              color: $brand-blue;
            }
          }
        }
      }
    }
    img {
      max-height: 100px;
      padding-bottom: 15px;
    }
  }
}
</style>
