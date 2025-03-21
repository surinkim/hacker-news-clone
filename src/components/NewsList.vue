<template>
  <div class="news-list">
    <ul>
      <li v-for="(news, index) in newsList" :key="index" class="news-item">
        <div class="news-rank">{{ index + 1 }}.</div>
        <div class="news-details">
          <a :href="news.url" target="_blank" class="news-title">{{ news.title }}</a>
          <span class="news-source"> ({{ news.source }})</span>
          <p class="news-summary">{{ news.summary }}</p>
          <div class="news-meta">
            <span>{{ news.points }} points by {{ news.author }} {{ news.time }} ago | </span>
            <a href="#" class="news-link">hide</a> | <a href="#" class="news-link">past</a> | <a href="#" class="news-link">discuss</a>
          </div>
        </div>
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
          summary: 'This is a summary of dummy news 1.',
          source: 'example.com',
          points: 1,
          author: 'user1',
          time: '1 minute'
        },
        {
          title: 'Dummy News 2',
          url: 'https://example.com/news2',
          summary: 'This is a summary of dummy news 2.',
          source: 'example.com',
          points: 1,
          author: 'user2',
          time: '1 minute'
        },
        {
          title: 'Dummy News 3',
          url: 'https://example.com/news3',
          summary: 'This is a summary of dummy news 3.',
          source: 'example.com',
          points: 1,
          author: 'user3',
          time: '1 minute'
        }
      ]
    };
  }
};
</script>

<style scoped>
.news-list {
  max-width: 800px;
  margin: 2rem auto;
  padding: 0 1rem;
}
.news-item {
  display: flex;
  align-items: flex-start;
  padding: 1rem;
  border-bottom: 1px solid #e0e0e0;
}
.news-rank {
  font-size: 1.25rem;
  font-weight: bold;
  margin-right: 1rem;
  color: #333333;
}
.news-details {
  flex: 1;
}
.news-title {
  font-size: 1.25rem;
  font-weight: bold;
  color: #007bff;
  text-decoration: none;
  transition: color 0.3s ease;
}
.news-title:hover {
  color: #0056b3;
}
.news-source {
  font-size: 0.875rem;
  color: #828282;
}
.news-summary {
  margin: 0.5rem 0;
  color: #333333;
}
.news-meta {
  font-size: 0.875rem;
  color: #828282;
}
.news-link {
  color: #007bff;
  text-decoration: none;
  transition: color 0.3s ease;
}
.news-link:hover {
  color: #0056b3;
}
</style>
