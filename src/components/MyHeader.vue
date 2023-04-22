<template>
  <div class="container">
    <section class="user">
      <img src="../assets/avatar.png" alt="Imagem de perfil" class="picture" />
      <p class="name">Lilia</p>
    </section>
    <section class="input">
      <input class="inputText" type="text" placeholder="procure aqui ..." />
      <button class="search">
        <img src="@/assets/search.png" alt="Ícone de pesquisa" />
      </button>
    </section>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>
.container {
  background: #13111B;
  max-height: 84px;
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #292730;
}

.user {
  display: flex;
  align-items: center;
}

.picture {
  margin: 16px 0 18px 32px;
}

.name {
  color: #FFFFFF;
  font-weight: 600;
  font-size: 18px;
  line-height: 24px;
}

.input {
  display: flex;
  margin: 17px 44px 17px 0;

  position: absolute 0;
  background: #191622;
  box-shadow: 0px 2px 4px rgba(255, 121, 198, 0.25);
  border-radius: 4px;
}

.inputText {
  font-family: Rubik;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;

  width: 363px;
  height: 50px;
  border-radius: 4px;
  background-color: #191622;
  color: #292730;
  border: none;
  padding: 16px;
  box-shadow: 0px 2px 4px rgba(255, 121, 198, 0.25);

  display: flex;
  align-items: center;
  text-transform: lowercase;
}

textarea:focus,
input:focus {
  box-shadow: 0 0 0 0;
  outline: 0;
  color: #fff;
}

.search {
  color: #ff79c6;
  width: 50px;
  background-color: transparent;
  border: none;
  margin-left: -60px;
}
</style>