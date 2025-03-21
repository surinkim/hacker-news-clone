<template>
  <div>
    <ul>
      <li v-for="(news, index) in newsList" :key="index">
        <span>{{ index + 1 }}. </span>
        <a :href="news.url" target="_blank">{{ news.title }}</a>
        <p>{{ news.summary }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newsList: [
        {
          title: 'Dummy News 1',
          url: 'https://example.com/news1',
          summary: 'This is a summary of dummy news 1.'
        },
        {
          title: 'Dummy News 2',
          url: 'https://example.com/news2',
          summary: 'This is a summary of dummy news 2.'
        },
        {
          title: 'Dummy News 3',
          url: 'https://example.com/news3',
          summary: 'This is a summary of dummy news 3.'
        }
      ]
    };
  }
};
</script>

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin-bottom: 1rem;
}

a {
  text-decoration: none;
  color: #0000ff;
}

p {
  margin: 0.5rem 0 0;
}
</style>
