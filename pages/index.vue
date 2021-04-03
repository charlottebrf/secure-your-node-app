<template>
  <section class="container">
    <div>
       <nav-bar/>
      <h1 class="title">
        Secure your Node apps
      </h1>
      <!-- <div class="links">
      <a class="button--green">
      <NuxtLink to="/javascript">Javascript</NuxtLink>
      </a>
       <a class="button--green">
      <NuxtLink to="/secure-code-reviews">Secure Code Reviews</NuxtLink>
       </a>
      </div>
    </div>
    <a href="https://nuxtjs.org">More about the author</a> -->
    </div>
  </section>
</template>

<script>
// a page imports a component to be rendered
  import NavBar from "~/components/NavBar.vue";
// exports itself & whatever components it is using
export default {
  components: {
     NavBar,
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

