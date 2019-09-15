<template>
  <main class="home-content">
    <p>
       Lorem ipsum dolor sit amet, consectetur adipisicing elit,
       sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
       Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
       nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
       esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
       sunt in culpa qui officia deserunt mollit anim id est laborum.
    </p>
    <p>
       Lorem ipsum dolor sit amet, consectetur adipisicing elit,
       sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
       Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
       nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
       esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
       sunt in culpa qui officia deserunt mollit anim id est laborum.
    </p>
    <p>
       Lorem ipsum dolor sit amet, consectetur adipisicing elit,
       sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
       Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
       nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
       esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
       sunt in culpa qui officia deserunt mollit anim id est laborum.
    </p>
  </main>
</template>

<script>

export default {
  name: 'home',
  metaInfo: {
    title: 'This is my home page',
    titleTemplate: null,
    meta: [
      { name: 'keywords', content: 'learn vue, javascript, lorem ipsum' },
      { name: 'author', content: 'Mateusz S' },
      { name: 'description', content: 'Strona testowa poświęcona nauce freameworka Vue' },
    ]
  }
}
</script>

<style>
.home-content {
  padding: 0 10%;
  display: flex;
  flex-direction: column;
}
p {
  margin:10px;
}
</style>
