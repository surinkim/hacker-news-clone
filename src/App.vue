<template>
  <div id="app">
    <Header />
    <NewsList />
    <!-- 다른 컴포넌트들 -->
  </div>
</template>

<script>
import Header from './components/Header.vue';
import NewsList from './components/NewsList.vue';

export default {
  name: 'App',
  components: {
    Header,
    NewsList,
  },
};
</script>

<style>
/* 전역 스타일 */
body {
  font-family: Arial, sans-serif;
  background-color: #f6f6ef;
  color: #333;
}
</style>
