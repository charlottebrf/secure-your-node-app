<template>
  <div>
    <h1>Fetching latest DevTo articles on security</h1>
    <ul>
      <li v-for="article in articles" :key="article.title">
        <!-- todo: how use internal links well -->
        <!-- <NuxtLink :to="{ name: 'articles-slug', params: { slug: article.slug } }"> -->
        <h1>{{ article.title }}</h1>
        <p>{{ article.description }}</p>
        <a>{{ article.url }}</a>
        <!-- </NuxtLink> -->
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  //:todo understand why doesn't this work?
  // async asyncData({ $http }) {
  //   const articles = await $http.$get('https://dev.to/api/articles?per_page=3&tag=security')
  //   console.log('articles', articles)
  //   return { articles }
  // },

  data() {
    return {
      articles: []
    };
  },
  async fetch() {
    this.articles = await fetch(
      "https://dev.to/api/articles?per_page=3&tag=security"
    ).then(res => res.json());
  }
};
</script>
