<template>
  <header>
    <div class="logo">
      <img src="/path/to/logo.png" alt="Site Logo" />
      <h1>Hacker News</h1>
    </div>
    <nav>
      <ul>
        <li><a href="#/new">New</a></li>
        <li><a href="#/past">Past</a></li>
        <li><a href="#/comments">Comments</a></li>
        <li><a href="#/ask">Ask</a></li>
        <li><a href="#/show">Show</a></li>
        <li><a href="#/jobs">Jobs</a></li>
        <li><a href="#/submit">Submit</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.logo {
  display: flex;
  align-items: center;
}

.logo img {
  height: 40px;
  margin-right: 1rem;
}

.logo h1 {
  font-size: 1.5rem;
  color: #333333;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

nav a {
  text-decoration: none;
  color: #333333;
  font-weight: 500;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #007bff;
}
</style>
