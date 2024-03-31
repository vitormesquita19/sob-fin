<script setup></script>

<template>
  <section class="header">
    <img class="logo" src="../assets/logo.svg" alt="App logo" />
    <div class="logo-title">
      <h2>SOBREVIVÊNCIA FINANCEIRA</h2>
    </div>
  </section>
  <section class="hero">
    <div class="hero-title">
      <h2>Escolha uma das trilhas abaixo para continuar:</h2>
    </div>
    <div class="card-grid">
      <div class="card">
        <div class="card-text">
          <h3>Trilha 1</h3>
          <p>Descrição trilha</p>
        </div>
        <div class="card-icon">
          <img src="../assets/money.svg" alt="Trilha bloqueada" />
        </div>
      </div>
      <div class="card">
        <div class="card-text">
          <h3>Trilha 2</h3>
          <p>Descrição trilha</p>
        </div>
        <div class="card-icon">
          <img src="../assets/money.svg" alt="Trilha bloqueada" />
        </div>
      </div>
      <div class="card">
        <div class="card-text">
          <h3>Trilha 3</h3>
          <p>Descrição trilha</p>
        </div>
        <div class="card-icon">
          <img src="../assets/money.svg" alt="Trilha bloqueada" />
        </div>
      </div>
      <div class="card">
        <div class="card-text">
          <h3>Trilha 4</h3>
          <p>Descrição trilha</p>
        </div>
        <div class="card-icon">
          <img src="../assets/money.svg" alt="Trilha bloqueada" />
        </div>
      </div>
      <div class="card">
        <div class="card-text">
          <h3>Trilha 5</h3>
          <p>Descrição trilha</p>
        </div>
        <div class="card-icon">
          <img src="../assets/money.svg" alt="Trilha bloqueada" />
        </div>
      </div>
      <div class="card">
        <div class="card-text">
          <h3>Trilha 6</h3>
          <p>Descrição trilha</p>
        </div>
        <div class="card-icon">
          <img src="../assets/money.svg" alt="Trilha bloqueada" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.header {
  top: 0;
  left: 0;
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  z-index: 1000;
}
.logo-title {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-size: 1.25rem;
}
.logo {
  height: 75px;
  margin-right: 10px;
}
.hero {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: rem 0;
}
.hero-title {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 2rem 0;
  font-size: 1rem;
}
.card-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 0 80px;
}
.card {
  flex: 0 0 calc(33.3333% - 40px);
  margin-bottom: 40px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.card:hover {
  background-color: #f3f3f3;
  cursor: pointer;
  border: 1px solid #000;
}
.card-text {
  flex: 0 0 70%;
}
.card-icon {
  flex: 0 0 30%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.card-icon img {
  width: 50px;
}
@media (max-width: 768px) {
  .logo {
    height: 50px;
  }
  .logo-title {
    font-size: 1rem;
  }
  .hero-title {
    font-size: 0.75rem;
  }
  .card-grid {
    padding: 0 20px;
  }
  .card {
    flex: 0 0 100%;
    margin-bottom: 20px;
  }
}
</style>
