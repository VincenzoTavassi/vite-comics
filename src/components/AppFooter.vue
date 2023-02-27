<script>
export default {};
</script>

<template>
  <footer>
    <div class="footer-bg-image">
      <div class="container">
        <nav class="col-4">
          <div class="col-33">
            <h2>DC COMICS</h2>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h2>SHOP</h2>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
            </ul>
          </div>
          <div class="col-33">
            <h2>DC</h2>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
          </div>
          <div class="col-33">
            <h2>SITES</h2>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
            </ul>
          </div>
        </nav>
      </div>
      <div class="sign-up-bg">
        <div class="container">
          <div class="sign-up">
            <button type="button" class="btn">SIGN UP NOW!</button>
            <div class="follow-icons">
              <h2>FOLLOW US</h2>
              <img src="../assets/img/footer-facebook.png" alt="" />
              <img src="../assets/img/footer-periscope.png" alt="" />
              <img src="../assets/img/footer-pinterest.png" alt="" />
              <img src="../assets/img/footer-twitter.png" alt="" />
              <img src="../assets/img/footer-youtube.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
@use "../assets/scss/mixins.scss" as *;

footer {
  background-color: black;
  padding-bottom: 50px;
}

.footer-bg-image {
  background-image: url("../assets/img/footer-bg.jpg");
  .container {
    max-width: 1200px;
    margin: 0 auto;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-position-x: right;
    background-position-y: center;
    background-repeat: no-repeat;
  }
}

.sign-up-bg {
  background-color: #333;
  .container {
    background-image: none;
  }
}

.sign-up {
  @include flex-center;
  justify-content: space-between;
  padding: 30px 0;
  .btn {
    padding: 15px;
    border: 2px solid #0c7cec;
    background-color: transparent;
    color: white;
    text-transform: uppercase;
    font-size: 1rem;
    font-weight: bolder;
    cursor: pointer;
    &:hover {
      background-color: white;
      color: #0c7cec;
    }
  }
  .follow-icons {
    @include flex-center;
    h2 {
      color: #0c7cec;
      display: inline-block;
      margin-right: 1rem;
    }
    img {
      margin-right: 1rem;
    }
  }
}

h2 {
  color: white;
  font-weight: bolder;
  font-size: 1.2rem;
  margin: 10px 0;
}

.col-4 {
  width: 40%;
  @include flex-center;
  align-items: flex-start;
  padding: 50px 0;
  ul {
    list-style-type: none;
    li {
      a {
        text-decoration: none;
        color: gray;
        font-size: 0.8rem;
        &:hover {
          color: #0c7cec;
        }
      }
    }
  }
}

.col-33 {
  width: calc(100% / 3);
}
</style>
