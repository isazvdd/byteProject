<template>
  <div class="container">
    <MySplash />
  </div>
</template>

<script>
import MySplash from "@/pages/MySplash.vue"

export default {
  components: {
    MySplash,
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
}
</style>