<script setup></script>

<template>
  <div class="app">
    <header>
      <div>My blog</div>
      <!--<nav class="nav">
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/about">About</NuxtLink>
        <NuxtLink to="/products">Products</NuxtLink>
      </nav>-->
    </header>
    <div class="body">
      <div class="sidebar">
        <li>
          <NuxtLink to="/">首頁</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">關於我</NuxtLink>
        </li>
        <li>
        <NuxtLink to="/game">遊戲</NuxtLink>
        </li>

      </div>
      <div class="main-container">
        <slot>This is where products page contents will be rendered</slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
.app {
  border: 2px solid darkseagreen;
}

header {
  background: #c4c2c2;
  padding: 0.4rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.body {
  display: flex;
}

.sidebar {
  display: flex;
  flex-direction: column;
  padding: 20px;
  width: 200px;
  background-color: #f4f4f4;
  text-align: left;
  height: 100vh;
}

.nav {
  display: flex;
  justify-content: flex-end;
  gap: 2rem;
}

footer {
  padding: 0.4rem 0;
  text-align: center;
  background: #999393;
}

.footer__nav {
  padding: 0 2rem;
  text-align: left;
  display: flex;
  justify-content: flex-start;
  gap: 2rem;
}

.router-link-exact-active {
  color: greenyellow;
}

</style>