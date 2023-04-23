<template>
  <div>
    <div class="container">
      <input type="text" class="input" placeholder="escreva aqui sua duvida ou problema..." />
      <button class="sendIcon">
        <img src="@/assets/send.png" alt="Ícone de enviar" />
      </button>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;

  background: #191622;
  border-radius: 4px;
  margin: 18px 33px auto 32px;
}

.input {
  height: 77px;
  width: 95%;
  max-width: 95%;
  background: #191622;
  border: none;
  padding: 30px 0 30px 25px;
}

.input::placeholder {
  font-weight: 500;
  font-size: 18px;
  color: #292730;
}

textarea:focus,
input:focus {
  box-shadow: 0 0 0 0;
  outline: 0;
  color: #fff;
}

.sendIcon {
  height: 77px;
  width: 50px;
  color: #FF79C6;
  border: none;
  background-color: transparent;
  margin-left: -65px;
}
</style>