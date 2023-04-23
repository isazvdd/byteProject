<template>
  <div class="container">
    <main>
      <router-view> </router-view>
    </main>
  </div>
</template>

<script>
export default {
  methods: {
    switchScreen() {
      setTimeout(() => {
        this.$router.push("/forum");
      }, 2000)
    },
  },
  mounted() {
    this.switchScreen();
  },
}
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  font-family: "Rubik", sans-serif;
  background-color: #13111B
}
</style>