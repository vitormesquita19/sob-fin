<script setup>
import Splash from "../components/Splash.vue";
import { ref } from "vue";

const isSplash = ref(true);

setTimeout(() => {
  isSplash.value = false;
}, 2000);
</script>

<template>
  <Splash v-if="isSplash" />
  <section class="login-container">
    <div class="mini-logo">
      <img src="../assets/logo.svg" alt="App logo" />
      <div class="mini-logo-title">
        <h2>SOBREVIVÊNCIA</h2>
        <h2>FINANCEIRA</h2>
      </div>
    </div>
    <div class="login-form">
      <form>
        <input type="text" placeholder="E-mail" />
        <input type="password" placeholder="Senha" />
        <router-link to="/home">
          <button type="submit">Entrar</button>
        </router-link>
      </form>
      <div class="additional-options">
        <div class="stay-connected">
          <input type="checkbox" />
          <label for="remember-me">Lembre-me</label>
        </div>
        <a href="#" class="register">Criar Conta</a>
      </div>
      <div class="breaker">
        <div class="left-line"></div>
        <div class="or">ou</div>
        <div class="right-line"></div>
      </div>
      <div class="sso-login">
        <button class="facebook">
          <img src="../assets/facebook.svg" alt="Facebook logo" />
          <span>Entrar com Facebook</span>
        </button>
        <button class="google">
          <img src="../assets/google.svg" alt="Google logo" />
          <span>Entrar com Google</span>
        </button>
      </div>
      <div class="forgot-pwd">
        <a href="#">Esqueceu a senha? Toque aqui para recuperar!</a>
      </div>
    </div>
  </section>
</template>

<style scoped>
.login-container {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
.mini-logo {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  margin: 0 auto 2rem;
}
.mini-logo-title {
  display: flex;
  justify-content: center;
  align-items: start;
  flex-direction: column;
  font-size: 1.25rem;
}
.mini-logo-title h2 {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 2px;
}
.mini-logo img {
  width: 100px;
}
.login-form {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  margin: 0 auto;
}
.login-form form {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.login-form input[type="text"],
.login-form input[type="password"] {
  width: 300px;
  height: 40px;
  margin: 5px;
  padding: 5px;
  padding-left: 15px;
  border: 1px solid #ccc;
  border-radius: 30px;
  background: #d6d6d6;
}
.login-form input::placeholder {
  color: #fff;
  font-size: 1rem;
}
.login-form button[type="submit"] {
  width: 300px;
  height: 40px;
  margin: 5px;
  padding: 5px;
  border: 1px solid #ccc;
  border-radius: 30px;
  background-color: #090b15ae;
  font-size: 1rem;
  color: #fff;
}
.login-form button:hover {
  background-color: #ccc;
}
.additional-options {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
  width: 100%;
}
.stay-connected {
  display: flex;
  justify-content: start;
  align-items: center;
  flex-direction: row;
  width: 50%;
  gap: 0.5em;
  margin: 5px;
  padding: 5px;
}
.register {
  display: flex;
  justify-content: end;
  align-items: center;
  flex-direction: row;
  width: 50%;
  margin: 5px;
  padding: 5px;
  text-decoration: none;
  color: #000;
}
.breaker {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  width: 100%;
  margin: 5px;
  padding: 5px;
}
.left-line,
.right-line {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  width: 45%;
  height: 3%;
  background-color: #000;
}
.or {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  width: 10%;
  margin: 0 5px;
  padding: 5px;
  font-size: 1rem;
  color: #000;
}
.sso-login {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  margin: 5px;
  padding: 5px;
}
.facebook,
.google {
  display: flex;
  justify-content: start;
  align-items: center;
  gap: 5px;
  width: 175px;
  height: 40px;
  margin: 5px;
  padding: 5px;
  border: 2px solid #000;
  border-radius: 30px;
  background-color: #fff;
  font-size: 0.8rem;
  color: #000;
}
.facebook img,
.google img {
  width: 25px;
  height: 25px;
  margin-right: 5px;
}
.sso-login button:hover {
  background-color: #ccc;
}
.forgot-pwd {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  width: 100%;
  margin: 5px;
  padding: 5px;
  padding-top: 1rem;
}
.forgot-pwd a {
  text-decoration: none;
  color: #000;
}
</style>
