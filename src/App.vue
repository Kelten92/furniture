<template>
  <div id="app">
    <new-navbar/>
    <new-header/>
    <router-view/>
  </div>
</template>

<style>
html,body {
  margin: 0;
}
body {
  background: #ebebeb;
}
#app {
  font-family: 'Mukta', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2E2E2E;
  background: #fff;
  position: relative;
  overflow-x: hidden;
}
@media (min-width:500px) {
  #app {
    margin:5% 10%;
    border-radius: 5px;
    -webkit-box-shadow: 0px 0px 40px 0px rgba(0,0,0,0.15);
    -moz-box-shadow: 0px 0px 40px 0px rgba(0,0,0,0.15);
    box-shadow: 0px 0px 40px 0px rgba(0,0,0,0.15);
  }
}
</style>

<script>
// @ is an alias to /src
import NewHeader from '@/components/NewHeader.vue'
import NewNavbar from '@/components/NewNavbar.vue'

export default {
  name: 'nav',
  components: {
    NewNavbar,
    NewHeader,
  },
  metaInfo: {
    title: 'Default Title',
    titleTemplate: '%s | My Awesome Webapp'
  },
}
</script>
