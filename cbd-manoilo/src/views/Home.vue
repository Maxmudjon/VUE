<template>
  <div class="home">
      <div class="home__top-panel">
        <nav class="home__nav">
          <a href="#" class="home__nav-links">HOME</a>
          <a href="#" class="home__nav-links">PRODUCTS</a>
          <a href="#" class="home__nav-links">FAQS</a>
          <a href="#" class="home__nav-links">CONTACT US</a>
        </nav>
        <div class="home__logo">
          <a href="#">CBD</a>
        </div>
        <div class="home__user-buttons">
          <div class="home__link-wrapper"><a href="#" class="home__btn-links">LOGIN</a></div>
          <div class="home__link-wrapper"><a href="#" class="home__btn-links">SEARCH</a></div>
         <div class="home__link-wrapper"> <a href="#" class="home__btn-links">CART (0)</a></div>
        </div>
      </div>
      <div class="home__content">
        <h1 class="home__title">Enhancing Life  Excelling in Care</h1>
        <h2 class="home__subtitile"> Choose Wisely. Choose CBD.</h2>
        <div class="home__btn"></div>

      </div>
  </div>
</template>

<script>


export default {
  name: 'Home',
  components: {
    
  }
}
</script>
<style lang="scss">
@import '../styles/core/vars.scss';
.home {
  min-height: 100vh;
  background-color: yellow;
  background-image: url('../assets/bg-header.png');
  color: white; 
  position: relative;
  font-weight: 400;
  font-family: $main-font;
  &__top-panel {
    position: absolute;
    top: 0;
    height: 7%;
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid $white;
  }
  &__nav {
    width: 25%;
    display: flex;
    justify-content: space-around;
    font-size: $nav-size;
  }
  &__logo {
    font-size: 30px;
  }
  &__user-buttons {
    font-size: $nav-size;
    display: flex;
    width: 25%;
    justify-content: space-around;
    height: 100%;
    align-items: center;
  }
 
  &__link-wrapper {
    height: 100%;
    width: 100%;
    border-left: 1px solid $white;
    display: flex;
    justify-content: center;
    align-items: center;
    
  }
  &__btn-links {
    width: 100%;
    
  }
  &__content {
    display: flex;
    margin: auto;
    flex-direction: column;
    height: 100vh;
    width: 60%;
    justify-content: center;
    align-items: flex-end;
  }
  &__title {
    font-size: $title-size;
    line-height: 75px;
    letter-spacing: 11px;
    text-transform: uppercase;
    text-align: right;
    width: 70%;
    margin-bottom: 15px;
  }
}
</style>