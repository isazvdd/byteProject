<template>
  <div>
    <h3>Dúvidas e Perguntas</h3>
    <div>
      <div class="questions" v-if="questions.length == 0">
        <h4 class="noQuestion">Nenhuma pergunta disponível ...T_T</h4>
      </div>
      <div class="cards" v-else v-for="question in questions" :key="question.question">
        <h4>{{ question.question }}</h4>
        <div class="iconsContainer">
          <button><img src="@/assets/heart.png" alt="ìcone de salvar" /></button>
          <button><img src="@/assets/like.png" alt="ìcone de like" /></button>
          <button><img src="@/assets/dislike.png" alt="ìcone de dislike" /></button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    questions: [],
  },
};
</script>

<style scoped>
h3 {
  color: #FF79C6;
  font-size: 22px;
  font-weight: 700;
  margin-left: 2rem;
  margin-bottom: 1.2rem;
  margin-top: 4.9rem;
}

.questions {
  font-size: 18px;
  font-weight: 700;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 67.4vh;
}

h4 {
  color: #FFFFFF;
  font-size: 18px;
  font-weight: 700;
  margin: 22px auto 24px 25px;
}

h4.noQuestion {
  display: flex;
  justify-content: center;
  align-items: center;
}

.cards {
  background: #191622;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 77px;
  max-width: 90%;
  padding: 22px auto 24px 25px;
  margin: auto;
  margin-bottom: 20px;
  border-radius: 4px;

}

.iconsContainer {
  background: #292730;
  display: flex;
  flex-direction: row;
  border-radius: 0px 4px 4px 0px;
  height: 77px;
  padding: 10px;
}

button {
  color: #FF79C6;
  background-color: transparent;
  border: none;
  padding: 5px;
  cursor: pointer;
}
</style>