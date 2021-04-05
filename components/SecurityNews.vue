<template>
  <div>
    <h1>Fetching Dev to </h1>
    <ul>
      <li v-for="article in articles" :key="article.title">
        <!-- <NuxtLink :to="{ name: 'articles-slug', params: { slug: article.slug } }"> -->
         {{ article.title }}
          {{ article.description }}
          {{ article.url }}
        <!-- </NuxtLink> -->
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  async asyncData({ $http }) {
    const articles = await $http.$get('https://dev.to/api/articles?per_page=3&tag=security')
    console.log('articles', articles)
    return { articles }
  }
}
</script>