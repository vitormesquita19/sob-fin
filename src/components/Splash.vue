<script setup></script>

<template>
  <section class="splash-container">
    <div class="splash-logo">
      <img src="../assets/logo.svg" alt="App logo" />
      <div class="splash-logo-title">
        <h2>SOBREVIVÊNCIA</h2>
        <h2>FINANCEIRA</h2>
      </div>
    </div>
    <div class="splash-loading"></div>
    <div class="splash-footer-logo">
      <img src="../assets/xpe-logo.svg" alt="Institution logo" />
    </div>
  </section>
</template>

<style scoped>
.splash-container {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}

.splash-logo {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin: 0 auto 2rem;
}

.splash-logo img {
  width: 150px;
}

.splash-logo-title {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-size: 1.25rem;
}

.splash-loading {
  border: 5px solid #f3f3f3;
  border-top: 5px solid #000;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  animation: spin 2s linear infinite;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

.splash-footer-logo {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 2rem;
}

.splash-footer-logo img {
  width: 150px;
}
</style>
