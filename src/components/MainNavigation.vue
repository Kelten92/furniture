<template>
  <nav class="main-navigation">
    <!-- <span class="hamburger">&#9776;</span> -->
    <ul class="link-list">
      <li class="list-item">
        <router-link to="/">Home</router-link>
      </li>
      <li class="list-item">
        <router-link to="/">About</router-link>
      </li>
      <li class="list-item">
        <router-link to="/product-page">Product</router-link>
      </li>
      <li class="list-item">
        <router-link to="/">Contact</router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
}
</script>

<style scoped>
.main-navigation {
  width: 100%;
  background: #66b9bf;
  color: #fff;
  padding: 15px 10%;
  font-size: 14px;
}
.link-list {
  padding: 0;
  display:flex;
  align-items: center;
  list-style: none;
  justify-content: flex-end;
}
.list-item a{
  text-decoration: none;
  color: #fff;
  text-transform: uppercase;
  margin:10px 20px;
  cursor: pointer;
  transition: .7s;
}
.list-item a:hover {
  color: #ddd;
}
</style>
