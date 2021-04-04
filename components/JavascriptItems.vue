<template>
  <div>
    <div v-for="item in items" :key="item.title">
      <item
        :title="item.title"
        :description="item.description"
        :url="item.url"
      ></item>
    </div>
  </div>
</template>

<script>
import Item from "~/components/Item.vue";

export default {
  components: { Item },
  data() {
    return {
      items: [
        {
          title: "JavaScript security 101",
          url: "https://dev.to/charlottebrf_99/javascript-security-101-2lag",
          description: `Run down of what was learnt on JavaScript Security: Best Practices course by Marcin Hoppe .`
        },
        {
          title: "Snyk JavaScript security",
          url: "https://snyk.io/learn/javascript-security",
          description: `Top 8 JS security vulnerabilities.`
        },
        {
          title: "OWASP",
          url: "https://cheatsheetseries.owasp.org/cheatsheets/Third_Party_Javascript_Management_Cheat_Sheet.html",
          description: `OWASP third party JS management cheat sheet".`
        }
      ]
    };
  }
};
</script>
