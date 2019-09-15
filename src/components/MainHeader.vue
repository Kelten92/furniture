<template>
  <header class="main-header">
    <div class="content-wrapper">
      <div class="call-to-action">
        <h1 class="title">Random call to action header</h1>
        <p class="descryption">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit,
          sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        </p>
      </div>
      <div class="img-content">
        <picture>
          <source srcset="../assets/hero.jpg" class="hero-img" media="(min-width: 401px)">
          <source srcset="../assets/hero-sm.jpg" class="hero-img" media="(max-width: 400px)">
          <img src="../assets/hero.jpg" class="hero-img" alt="hero-image">
        </picture>
      </div>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
.main-header {
  padding: 5% 10%;
}
.content-wrapper {
  display:flex;
  justify-content: space-around;
}
.call-to-action {
  flex: 2;
  margin: 0 15px;
}
.hero-img {
  display: block;
  width: 100%;
  height: auto;
}
.img-content {
  flex: 3;
}
.descryption {
  font-size: 16px;
}
</style>
