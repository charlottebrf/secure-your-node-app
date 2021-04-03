<template>
<div>
    <div v-for="item in items" :key="item.title">
      <item :title="item.title" :description="item.description" :url="item.url"></item>
  </div>
  </div>
</template>

<script>
import Item from '~/components/Item.vue'

export default {
    components: { Item },
    data() {
    return {
      items: [
        {
          title: 'blah',
          url: 'https://s3-us-west-2.amazonaws.com/s.cdpn.io/28963/moscow.svg',
          description: `Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.`
        },
        {
          name: 'blurghh',
          img: 'https://s3-us-west-2.amazonaws.com/s.cdpn.io/28963/paris1.svg',
          desc: `Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.`
        },
         {
          name: 'blahhh',
          img: 'https://s3-us-west-2.amazonaws.com/s.cdpn.io/28963/rome.svg',
          desc: `Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.`
        },
      ],
    }
  },
  }
</script>
