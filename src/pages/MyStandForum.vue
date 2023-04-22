<template>
  <div class="container">
    <MyHeader />
    <section class="mainSection">
      <div class="questionContainer">
        <MySendInput />
        <!-- <Question :questions="questions" /> -->
      </div>
      <div>
        <!-- <Sidebar :questions="questions" /> -->
      </div>
    </section>
  </div>
</template>

<script>
import MyHeader from "@/components/MyHeader.vue";
import MySendInput from "@/components/MySendInput.vue";

export default {
  components: {
    MyHeader,
    MySendInput,
  },
};
</script>

<style scoped>
/* .container {
  height: 100vh;
  background-color: #1E1E1E;
} */
</style>