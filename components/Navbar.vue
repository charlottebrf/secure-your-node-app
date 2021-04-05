<template>
  <div class="nav">
    <nav>
      <nuxt-link class="nav-item router-link-exact-active" to="/"
        >Home</nuxt-link
      >
      <nuxt-link class="nav-item router-link-exact-active" to="/javascript"
        >Javascript</nuxt-link
      >
      <nuxt-link
        class="nav-item router-link-exact-active"
        to="/secure-code-reviews"
        >Secure Code Reviews</nuxt-link
      >
       <nuxt-link
        class="nav-item router-link-exact-active"
        to="/security-news"
        >Security News</nuxt-link
      >
    </nav>
  </div>
</template>

<style scoped>
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
}
.nav .nav-item {
  box-sizing: border-box;
  margin: 0 5px;
  color: rgba(0, 0, 0, 0.5);
  text-decoration: none;
}
.nav .nav-item.router-link-exact-active {
  color: #39b982;
  border-bottom: solid 2px #39b982;
}
.nav a {
  display: inline-block;
}
</style>
