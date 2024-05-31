<script setup lang="ts">
const topics = [
  {
    date: '2024/06/12',
    title: '◯◯を実施しました。',
  },
  {
    date: '2024/05/20',
    title: 'XXXXをリリースしました！',
  },
  {
    date: '2024/05/13',
    title: 'XXのという雑誌に掲載されました。',
  },
];
</script>

<template>
  <dl class="news_container">
    <div class="news_list" v-for="topic in topics">
      <dt>{{ topic.date }}</dt>
      <dd>{{ topic.title }}</dd>
    </div>
  </dl>
</template>

<style scoped>
.news_list {
  display: flex;
  border-top: solid 1px #c8c8c8;
  > * {
    border-bottom: solid 1px #c8c8c8;
    padding: 16px;
    &:is(dt) {
      width: 20%;
    }
    &:is(dd) {
      width: 80%;
      margin: 0;
    }
  }
}
</style>
