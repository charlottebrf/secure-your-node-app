<template>
  <div class="smol-card-component ">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
    <!-- <a href={{ url }}><button>url</button></a> -->
    <a> {{ url }} </a>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: ["title", "description", "url"]
};
</script>

<style scoped>
.smol-flexbox-grid {
  --min: 10ch;
  --gap: 1rem;

  display: flex;
  flex-wrap: wrap;
  gap: var(--gap);
}
.smol-flexbox-grid > * {
  flex: 1 1 var(--min);
}

.smol-card-component {
  --img-ratio: 3/2;

  display: flex;
  flex-direction: column;
  box-shadow: 0 0 0.5rem rgba(0, 0, 0, 0.35);
  border-radius: 0.5rem;
  padding: 1rem;
}

/* Soon we can replace this with: gap: 1rem; */
.smol-card-component > * + * {
  margin-top: 1rem;
}

a {
  color: #39b982;
  border-bottom: solid 2px #39b982;
}

</style>
