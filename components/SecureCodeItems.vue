<template>
  <div>
    <div v-for="item in securecodeitems" :key="item.title">
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
      securecodeitems: [
        {
          title: "8 security code review best practices",
          url: "https://snyk.io/blog/secure-code-review",
          description: `Some quick tips for carrying out more secure code reviews`
        },
        {
          title: "OWASP code review guide",
          url: "https://owasp.org/www-pdf-archive/OWASP_Code_Review_Guide_v2.pdf",
          description: `A very long PDF which must have some gold in it somewhere (if you can find it)`
        },
        {
          title: "Security Code Reviews 101 series",
          url: "https://medium.com/@paul_io/security-code-review-101-a3c593dc6854",
          description: `Useful series focusing on how to ensure secure coding practices when doing code review`
        }
      ]
    };
  }
};
</script>
