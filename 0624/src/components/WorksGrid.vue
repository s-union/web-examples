<script setup lang="ts">
const items = [
  {
    title: 'タイトルA',
    description: 'テストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテスト',
    path: 'works1.jpg',
  },
  {
    title: 'タイトルB',
    description:
      'テストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテスト',
    path: 'works2.jpg',
  },
  {
    title: 'タイトルC',
    description: 'テストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテスト',
    path: 'works3.jpg',
  },
  {
    title: 'タイトルD',
    description: 'テストテスト',
    path: 'works4.jpg',
  },
  {
    title: 'タイトルE',
    description: 'テスト・テスト・テスト・テスト・テスト・テスト・テスト・テスト・テスト',
    path: 'works5.jpg',
  },
  {
    title: 'タイトルF',
    description:
      'テストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテストテスト',
    path: 'works6.jpg',
  },
];
</script>

<template>
  <div class="works_container">
    <div class="works_sub_container" v-for="item in items">
      <img :src="`/src/assets/works/${item.path}`" />
      <div>
        <h5>{{ item.title }}</h5>
        <span>{{ item.description }}</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.works_container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 16px;
}

.works_sub_container {
  display: grid;
  grid-template-rows: subgrid;
  grid-row: span 3;
  background-color: #f5f5f5;
  border-radius: 5%;
  overflow: hidden;
  & img {
    max-width: 100%;
  }
  & h5 {
    margin-block: 8px;
  }
  > div {
    padding-inline: 16px;
  }
}
</style>
