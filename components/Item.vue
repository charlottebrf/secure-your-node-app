<template>
  <div class="item">
    <h1>{{ title }}</h1>
      <p> {{ description }} </p>
      <a> {{ url }} </a>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: ['title', 'description', 'url'],
};
</script>

<style scoped>
.item {
  display: flex;
  flex-direction: column;
  width: 280px;
  height: 320px;
  justify-content: center;
  background: white;
  border: 1px solid #ddd;
  padding: 20px 20px;
  margin: 10px;
}
</style>
