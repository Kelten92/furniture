<template>
  <nav class="new-navbar">
    <div class="hamburger" @click="toggleMenu">
      <div class="line1"></div>
      <div class="line2"></div>
      <div class="line3"></div>
    </div>
    <div class="logo">Logo MS</div>
    <ul class="new-navbar__list">
      <li class="new-navbar__list__item"><router-link to="/">Home</router-link></li>
      <li class="new-navbar__list__item"><router-link to="/">About</router-link></li>
      <li class="new-navbar__list__item"><router-link to="/product-page">Product</router-link></li>
      <li class="new-navbar__list__item"><router-link to="/">Contact</router-link></li>
    </ul>
  </nav>
</template>

<script>
export default {
  data: () => {
    return {
      showMenu: false,
    }
  },
  methods: {
    toggleMenu: function() {
      let nav = document.querySelector('.new-navbar__list');
      let btn = document.querySelector('.hamburger');
      nav.classList.toggle('nav-active');
      btn.classList.toggle('btn-active');
    }
  }
}
</script>

<style scoped>
.new-navbar {
  overflow: hidden;
  background: white;
  border-bottom: .5px solid lightGrey;
  height: 10vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.new-navbar__list {
  background: #fff;
  list-style: none;
  display: flex;
  margin:0;
  padding:0;
  justify-content: space-around;
  width: 50%;
  flex-direction: column;
  position: absolute;
  z-index: 1;
  right:0;
  height: 90vh;
  top:10vh;
  align-items: center;
  transform: translateX(100%);
  transition: transform 0.5s cubic-bezier(0.21, 0.87, 0.32, 1.28);
}
.hamburger div {
  width: 25px;
  height: 3px;
  background: black;
  margin: 5px;
}
.nav-active {
  transform: translateX(0%);
}
.new-navbar__list__item {
  position: relative;
}
.new-navbar__list__item a {
  color: #2E2E2E;
  text-decoration: none;
  text-transform: uppercase;
  font-size: 14px;
  padding: 5px 0;
  display: block;
  vertical-align: middle;
}
.new-navbar__list__item a::before {
  content: '';
  display:block;
  border-top: 2px solid #000;
  border-bottom: 2px solid #000;
  position: absolute;
  top:0;
  left:0;
  width: 100%;
  height: 100%;
  transition: .6s;
  opacity: 0;
}
.new-navbar__list__item a:hover::before {
  opacity: 1;
}
.logo {
  text-transform: uppercase;
  letter-spacing: 5px;
  font-weight: bolder;
}
.line1, .line2, .line3 {
  transition: transform .4s ease;
}
.hamburger.btn-active > .line1 {
  transform: translateX(5px);
}
.hamburger.btn-active > .line2 {

}
.hamburger.btn-active > .line3 {
  transform: translateX(5px);
}

@media (min-width:500px) {
  .hamburger {
    display: none;
  }
  .new-navbar__list {
    transform: translateX(0);
    flex-direction: row;
    position: static;
    width: 35%;
    height: auto;
  }
}
</style>
