<template>
  <section class="info-tile">
    <img src="@/assets/hero-sm.jpg" class="tile-img">
    <div class="tile-title">
      <h2 class="number">01</h2>
      <div class="desc-wrapper">
        <h3 class="desc-title">Produkcja łóżek</h3>
        <p class="desc-subtitle">Lorem ipsum dolor sit amet</p>
      </div>
    </div>
    <p class="tile-paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Enim recusandae officia, voluptate! Error natus, veniam esse enim temporibus nihil autem.</p>
  </section>
</template>

<script>
export default {
  name: 'InfoTile',

}
</script>

<style scoped>
.info-tile {
  width:100%;
}
.tile-img {
  width: 100%;
  display: block;
  height: auto;
}
.tile-title {
  display: flex;
  width: 100%;
  justify-content: flex-start;
}
.number {
  font-size: 42px;
  margin: 10px;
  margin-left: 0;
  line-height: 0.8;
  border-bottom: 2px solid black;
}
.desc-wrapper {

}
.desc-title {
  margin: 10px;
  line-height: 0.9;
  text-transform: uppercase;
  font-weight: 500;
}
.desc-subtitle {
  font-size: 12px;
  margin: 5px 10px;
  line-height: 0.8;
}
.tile-paragraph {
  margin:0;
  font-size: 14px;
}
</style>
