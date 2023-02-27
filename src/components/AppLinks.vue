<script>
export default {};
</script>

<template>
  <section>
    <div class="container">
      <div class="action-link">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
        <span>Digital Comics</span>
      </div>
      <div class="action-link">
        <img src="../assets/img/buy-comics-merchandise.png" alt="" />
        <span>DC Merchandise</span>
      </div>
      <div class="action-link">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
        <span>Subscription</span>
      </div>
      <div class="action-link">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
        <span>Comic Shop Locator</span>
      </div>
      <div class="action-link">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
        <span>DC Power Visa</span>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use "../assets/scss/mixins.scss" as *;

section {
  background-color: #0c7cec;
  padding: 50px;
  color: white;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
  @include flex-center;
}

.action-link {
  @include flex-center;
  padding: 10px 0;
  width: calc(100% / 5);
  text-transform: uppercase;
  font-size: 0.9rem;
  img {
    margin-right: 1rem;
    max-height: 55px;
  }
}
</style>
