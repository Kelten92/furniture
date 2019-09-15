<template>
  <main class="product-page">
    <h1>Product Page</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    <div style="display:flex; width:100%;">
    <div v-for="item in items"><info-tile/></div>
  </div>
  </main>
</template>

<script>
import InfoTile from '@/components/InfoTile.vue';
export default {
  metaInfo: {
    title: 'My product page',
    titleTemplate: null
  },
  components: {
    InfoTile,
  },
  data: function(){
    return {
      items: ['1', '2'],
    }
  }
}
</script>

<style scoped>
.product-page {
  padding: 0 10%;
}
</style>
