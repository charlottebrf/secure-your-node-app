<template>
  <div>
    <navbar></navbar>
    <javascript-items></javascript-items>
  </div>
</template>

<script>
import JavascriptItems from "~/components/JavascriptItems.vue";
import Navbar from "~/components/Navbar.vue";

export default {
  components: { JavascriptItems, Navbar }
};
</script>
