<template>
  <div>
    <h1>Fetching latest DevTo articles on security</h1>
    <ul>
      <li v-for="article in articles" :key="article.title">
        <h1>{{ article.title }}</h1>
        <p>{{ article.description }}</p>
        <a>{{ article.url }}</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  async asyncData({ $http }) {
    const articles = await $http.$get(
      "https://dev.to/api/articles?per_page=3&tag=security"
    );
    return articles;
  }
};
</script>
