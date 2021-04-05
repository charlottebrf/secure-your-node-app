<template>
  <div>
    <navbar></navbar>
    <security-news></security-news>
  </div>
</template>

<script>
import Navbar from "~/components/Navbar.vue";
import SecurityNews from '../components/SecurityNews.vue';

export default {
  components: { SecurityNews, Navbar }
};
</script>
