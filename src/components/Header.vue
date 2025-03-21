<template>
  <header>
    <img src="/path/to/logo.png" alt="Site Logo" />
    <nav>
      <ul>
        <li><a href="#/new">New</a></li>
        <li><a href="#/past">Past</a></li>
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
  padding: 1rem;
  background-color: #f6f6ef;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 1rem;
}

nav a {
  text-decoration: none;
  color: #333;
}
</style>
