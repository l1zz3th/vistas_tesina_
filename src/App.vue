<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <h1 class="title">Inicia Sesion</h1>
<header>
    <img alt="Fondo" class="img-fondo" src="@/assets/images/fondo.jpg"  />

    <div class="form">
      
    <form action class="form" @submit.prevent="register">
      <label class="form-label" for="#email">Email:</label>
      <input
        v-model="email"
        class="form-input"
        type="email"
        id="email"
        required
        placeholder="Email"
      >
      <label class="form-label" for="#password">Password:</label>
      <input
        v-model="password"
        class="form-input"
        type="password"
        id="password"
        placeholder="Password"
      >
      <label class="form-label" for="#password-repeat">Repite la contraeña:</label>
      <input
        v-model="passwordRepeat"
        class="form-input"
        type="password"
        id="password-repeat"
        placeholder="Password"
      >
      <input class="form-submit" type="submit" value="Sign Up">
    </form>
    </div>
</header>

</template>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 {
  text-align: center;
  text-color: black;
	width: auto;
	height: auto;
	padding: 8px 8px 8px 8px;
	background: #ffebd2;
	border-color: #ffebd2;
	border-width: 1px;
	border-style: solid;
}


header{
  background-color: white;
  border: black;
  width:auto;
  height:auto;
}
.img-fondo {
  color: #fff;
  align-content: left;
}

.form {
  text-align: left;
  color: #da5526;
}

.tittle {
  text-align: center;

}



</style>
