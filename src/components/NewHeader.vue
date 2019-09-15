<template>
  <header class="main-header">
    <div class="header-text">
      <h1 class="call-to-action">Page call to <u>action</u> header</h1>
      <p class="more-info">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Odit ipsam assumenda, repudiandae ipsa dolore laudantium saepe beatae tenetur natus aspernatur voluptatum nostrum omnis, aliquam, iure.
      </p>
    </div>
    <carousel/>
  </header>
</template>

<script>
import Carousel from './Carousel.vue'
export default {
  components: {
    Carousel,
  }
}
</script>

<style scoped>
.main-header {
  padding: 5%;
}
.call-to-action {
  font-size: 30px;
  letter-spacing: 1px;
  line-height: 1.3;
  font-weight: 900;
  text-align: center;
}
.more-info {
  font-size: 16px;
  display: none;
}
.hero-img {
  display: block;
  width: 100%;
  height: auto;
}
.slide-wrapper {
  overflow: hidden;
  position: relative;
}
@media (min-width:500px) {
  .main-header {
    padding: 5% 10%;
    display: flex;
    align-items: center;
  }
  .header-text {
    flex: 1;
    margin: 25px;
  }
  .slider-wrapper {
    flex: 2.5;
  }
  .call-to-action {
    text-align: left;
    font-size: 42px;
  }
  .more-info {
    display: inline;
  }
}
</style>
