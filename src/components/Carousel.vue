<template>

    <transition-group tag="div" class="img-slider" name="slide">
        <div v-for="number in [currentImg]" v-bind:key="number">
          <img :src="imgList[Math.abs(currentImg) % imgList.length]"/>
        </div>
    </transition-group>

</template>

<script>
export default {
  data: function(){
    return {
      imgList: [
        require('@/assets/hero.jpg'), require('@/assets/hero.jpg'), require('@/assets/hero.jpg')
      ],
      currentImg: 0,
    }
  },
  mounted() {
  	setInterval(() => {
    	this.currentImg = this.currentImg + 1;
    }, 4000);
  },
  methods: {

  }
}
</script>

<style scoped>
.slide {
  overflow: hidden;
  position: relative;
}
.slide-leave-active,
.slide-enter-active {
  transition: 1s;
}
.slide-enter {
  transform: translate(100%, 0);
}
.slide-leave-to {
  transform: translate(-100%, 0);
}
.img-slider{
  overflow: hidden;
  position: relative;
  width: 100%;
  min-height: 200px;
}
.img-slider img {
  position: absolute;
  width: 110%;
}
@media (min-width:500px){
  .img-slider {
    flex: 2;
    min-height: 350px;
  }
}
</style>
