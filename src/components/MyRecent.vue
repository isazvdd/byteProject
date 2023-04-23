<template>
  <div class="container">
    <h3>Recentes</h3>
    <div>
      <div class="questions" v-if="questions.length == 0">
        <h4>Nenhuma pergunta disponível ...T_T</h4>
      </div>
      <div class="cards" v-else v-for="question in questions" :key="question.question">

        <h4>{{ question.question }}</h4>
        <div class="icons">
          <span>{{ question.name }}</span>
          <div>
            <button>
              <img src="@/assets/heart.png" alt="" />
            </button>
            <button><img src="@/assets/like.png" alt="" /></button>
            <button><img src="@/assets/dislike.png" alt="" /></button>
          </div>
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
.container {
  background: #191622;
  border-left: 1px solid #292730;
  width: 25%vw;
}

h3 {
  color: #FF79C6;
  font-size: 22px;
  font-weight: 700;
  margin-bottom: 16px;
  padding-left: 12px;
  padding-top: 16px;
}

.questions {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 18px;
  font-weight: 700;
  height: 87vh;
  margin-right: 22px;
  border-radius: 4px;
}

h4 {
  color: #FFFFFF;
  font-size: 18px;
  font-weight: 700;
  padding: 10px;
}

.cards {
  background: #13111b;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 95%;
  margin: auto;
  margin-bottom: 18px;
  border-radius: 4px;
}

.cards h4 {
  margin: 19px 18px 30px 23px;
}

.icons {
  background: #292730;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 62px;
  width: 100%;
  border-radius: 0px 0px 4px 4px;
}

span {
  color: #FF79C6;
  font-size: 18px;
  font-style: normal;
  font-weight: 600;
  margin: 20px auto 21px 18px
}

button {
  color: #FF79C6;
  background-color: transparent;
  width: 50px;
  border: none;
  cursor: pointer;
}
</style>