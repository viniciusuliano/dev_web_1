<template>
  <div class="header">
    <nav>
      <img class="logo" src="/src/assets/logo.png" alt="logo" />
      <div>
        <button class="lang-btn">
          <i class="fa-solid fa-globe"></i> Português
          <img src="/src/assets/down-icon.png" />
        </button>
        <button>Entrar</button>
      </div>
    </nav>

    <div class="header-content">
      <h1>Filmes, séries e muito mais, sem limites.</h1>
      <h3>Assista onde quiser. Cancele quando quiser.</h3>
      <p>
        Pronto para assistir? Insira seu e-mail para criar ou reiniciar sua assinatura.
      </p>
      <form action="#" class="email-signup">
        <input type="email" placeholder="Endereço de e-mail" required />
        <button type="submit">Vamos lá</button>
      </form>
    </div>
  </div>
</template>


<script>
export default {
  name: 'HeaderComponent',
};
</script>

<style scoped>
.header {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url(./src/assets/header-image.png);
  background-size: cover;
  background-position: center;
  padding: 10px 8%;
  position: relative;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 0;
}

.logo {
  width: 150px;
  cursor: pointer;
}

nav button {
  border: none;
  outline: none;
  background-color: #db0001;
  color: #fff;
  padding: 7px 20px;
  font-size: 12px;
  border-radius: 4px;
  margin-left: 10px;
  cursor: pointer;
}

.lang-btn {
  display: inline-flex;
  align-items: center;
  background: transparent;
  border: 1px solid #fff;
  padding: 7px 10px;
}

.lang-btn img {
  width: 10px;
  margin-left: 10px;
}

.fa-globe {
  color: #fff;
  width: 10px;
  margin-right: 10px;
}

.header-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  margin-top: 100px;
}

.header-content h1 {
  font-size: 60px;
  line-height: 70px;
  font-weight: 600;
  max-width: 650px;
}

.header-content h3 {
  font-weight: 400;
  margin-bottom: 20px;
}

.email-signup {
  background: #fff;
  border-radius: 4px;
  display: flex;
  align-items: center;
  margin-top: 30px;
  overflow: hidden;
}

.email-signup input {
  flex: 1;
  border: 0;
  outline: 0;
  margin-left: 20px;
}

.email-signup button {
  background-color: #db0001;
  border: none;
  outline: none;
  color: #fff;
  font-size: 16px;
  cursor: pointer;
  padding: 15px 30px;
}

@media only screen and (max-width: 600px) {
  .logo {
    width: 100px;
  }

  nav button {
    padding: 5px 10px;
  }

  nav .lang-btn {
    padding: 4px 8px;
  }

  .header-content {
    position: unset;
    transform: none;
    padding-top: 150px;
  }

  .header-content h1 {
    font-size: 30px;
  }

 .email-signup button {
    font-size: 12px;
    padding: 10px 15px;
  }
}
</style>
