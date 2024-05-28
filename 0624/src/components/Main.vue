<script setup lang="ts">
import WorksGrid from './WorksGrid.vue';
</script>

<template>
  <section id="about">
    <h2 class="section_title">About</h2>
    <p>
      AAAAAAAAAAAAAAAAAAAAAAAAAAABBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD
    </p>
    <ul>
      <li>これは</li>
      <li>テストの</li>
      <li>ウェブサイト</li>
      <li>です。</li>
    </ul>
  </section>
  <section id="works">
    <h2 class="section_title">Works</h2>
    <WorksGrid />
  </section>
</template>

<style scoped>
.section_title {
  text-align: center;
  font-size: 24px;
  padding-block: 16px;
}

section {
  width: 100%;
  padding-bottom: 80px;
}
</style>
