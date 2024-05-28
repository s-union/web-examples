<script setup lang="ts"></script>

<template>
  <header class="header">
    <h1>Hello Page!</h1>
    <nav>
      <ul class="header_nav">
        <li><a href="">About</a></li>
        <li><a href="">Works</a></li>
        <li><a href="">News</a></li>
        <li><a href="https://instagram.com">Instagram</a></li>
      </ul>
    </nav>
  </header>
  <img class="header_image" src="../assets/header.jpg" alt="ヘッダー画像" />
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-inline: 8px;
}

.header_nav {
  display: flex;
  & li {
    list-style-type: none;
    margin-left: 16px;
    & a {
      text-decoration: none;
      color: #333132;
      &:hover {
        opacity: 0.7;
      }
    }
  }
}

.header_image {
  width: 100vw;
  margin-inline: calc(50% - 50vw);
}
</style>
