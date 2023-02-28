<script>
export default {
  props: {
    image: String,
    title: String,
  },
};
</script>

<template>
  <div>
    <a href="#">
      <img :src="image" alt="" />
      <span>{{ title }}</span>
    </a>
  </div>
</template>

<style scoped>
span {
  color: white;
  text-transform: uppercase;
  font-size: 0.8rem;
  margin-top: 10px;
  font-weight: 200;
}

img {
  height: 170px;
}

a {
  display: flex;
  flex-direction: column;
  width: 170px;
}
</style>
