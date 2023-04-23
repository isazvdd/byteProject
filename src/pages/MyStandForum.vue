<template>
  <div class="container">
    <Header />
    <section>
      <div class="questions">
        <Search />
        <!-- <Recent /> -->
        <Question :questions="questions" />
      </div>
      <div>
        <Recent :questions="questions" />
      </div>
    </section>
  </div>
</template>

<script>
import Header from "@/components/MyHeader.vue";
import Search from "@/components/MySearch.vue";
import Recent from "@/components/MyRecent.vue";
import Question from "@/components/MyQuestion.vue";

export default {
  data() {
    return {
      questions: [
        {
          name: "Gustavo",
          question:
            "Não consigo mudar a versão do meu Node no linux, como faço?",
        },
        {
          name: "Luana",
          question: "Como salvar dados com o localHistory Vue3?",
        },
        {
          name: "Carlos",
          question: "Como conecta o firebase com Vue3?",
        },
        {
          name: "Isadora",
          question: "oi, vamo sair?",
        },

      ],
    };
  },
  components: {
    Header,
    Search,
    Recent,
    Question,
  },
};
</script>

<style scoped>
section {
  display: flex;
  justify-content: space-between;
}

.questions {
  width: 100%;
}
</style>