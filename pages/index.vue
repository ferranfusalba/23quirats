<template>
  <Header />
</template>

<script>
import Header from "@/components/Header.vue"

export default {
  name: 'IndexPage',
  components: {
    Header
  },
  data() {
    return {
      title: "Florí Design System"
    }
  },
  head() {
      return {
        title: this.title,
        meta: [
          // hid is used as unique identifier. Do not use `vmid` for it as it will not work
          {
            hid: 'description',
            name: 'description',
            content: 'My custom description'
          }
        ]
      }
    }
}
</script>
