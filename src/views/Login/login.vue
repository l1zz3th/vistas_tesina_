<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div class="contenedor">
    <h1 class="title">Inicia Sesion</h1>
    <Content>
      <img alt="Fondo" class="img-fondo" src="@/assets/images/fondo.jpg" />

      <div>
        <form action class="form">
          <label class="form-label" for="#email">Email:</label>
          <input
            v-model="email"
            class="form-input"
            type="email"
            id="email"
            required
            placeholder="Email"
          />
          <label class="form-label" for="#password">Password:</label>
          <input
            v-model="password"
            class="form-input"
            type="password"
            id="password"
            placeholder="Password"
          />

          <input class="form-submit" type="submit" value="Iniciar Sesion" />
        </form>
      </div>
    </Content>
  </div>
</template>

<style scoped>
.contenedor {
  background: white;
  width: 900px;
  height: 3rem auto;
  align-content: center;
  display: block; 
}
.content {
  display: flex;
  align-items: center;
  height: 80vh;
  margin: 0 auto;
  max-width: 1200px;
  width: 95%;
}

h1 {
  text-align: center;
  color: black;
  width: auto;
  height: 70px;
  padding: 8px 8px 8px 8px;
  background: #ffebd2;
  border-color: #ffebd2;
  border-width: 1px;
  border-style: solid;
}

.img-fondo {
  background-position: left left;
  background-size: cover;
  height: auto;
  width: auto;
  flex: 0 0 calc(60%);
  position: relative;
}

.tittle {
  text-align: center;
}
.form {
  margin: 3rem auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: auto;
  min-width: auto;
  max-width: auto;
  background: rgba(250, 253, 255, 0.9);
  border-radius: 5px;
  padding: 40px;
  box-shadow: 0 4px 10px 4px rgba(0, 0, 0, 0.3);
}
.form-label {
  width: 154px;
  height: 60px;
  color: #da5526;
  font-family: "Arial";
  font-size: large;
  text-align: left;
}

.form-input {
  padding: 10px 15px;
  border: 1px solid rgb(0, 0, 0);
  color: rgb(2, 2, 2);
}
.form-submit {
  background: #da810d;
  border: none;
  color: white;
  margin-top: 3rem;
  padding: 1rem 0;
  cursor: pointer;
}
.error {
  margin: 1rem 0 0;
  color: #ff4a96;
}
.button {
  width: 415px;
  height: 107px;
  padding: 8px 8px 8px 8px;
  box-shadow: 0px 5px 10px rgba(248, 95, 106, 0.23);
  background: #f68930;
  border-radius: 6px 6px 6px 6px;
}

@import url('https://fonts.googleapis.com/css2?family=Comfortaa&family=Libre+Franklin:wght@300&display=swap" rel="stylesheet');
</style>
