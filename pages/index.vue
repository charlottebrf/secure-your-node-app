<template>
  <section>
    <div>
      <nav-bar />
      <h1 class="title">
        Secure your Node apps
      </h1>
    </div>
  </section>
</template>

<script>
import NavBar from "~/components/NavBar.vue";
export default {
  components: {
    NavBar
  }
};
</script>

<style>
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>
