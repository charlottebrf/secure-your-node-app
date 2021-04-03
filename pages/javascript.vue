<template>
<div>
    <navbar></navbar>
    <items></items>
</div>
</template>

<script>
import Items from '~/components/Items.vue'
import Navbar from '~/components/Navbar.vue'

export default {
    components: { Items, Navbar }
  }
</script>
