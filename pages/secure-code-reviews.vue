<template>
  <div>
    <navbar></navbar>
    <secure-code-items></secure-code-items>
  </div>
</template>

<script>
import SecureCodeItems from "~/components/SecureCodeItems.vue";
import Navbar from "~/components/Navbar.vue";

export default {
  components: { SecureCodeItems, Navbar }
};
</script>
