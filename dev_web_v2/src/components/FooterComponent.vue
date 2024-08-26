<template>
  <div class="footer">
    <h2>Dúvidas? Ligue para 000-000-000-0000</h2>

    <div class="row">
      <div class="col">
        <a href="#">Perguntas Frequentes</a>
        <a href="#">Relações com Investidores</a>
        <a href="#">Privacidade</a>
        <a href="#">Teste de Velocidade</a>
      </div>
      <div class="col">
        <a href="#">Central de Ajuda</a>
        <a href="#">Carreiras</a>
        <a href="#">Preferências de Cookies</a>
        <a href="#">Avisos Legais</a>
      </div>
      <div class="col">
        <a href="#">Conta</a>
        <a href="#">Formas de Assistir</a>
        <a href="#">Informações Corporativas</a>
        <a href="#">Só na Netflix</a>
      </div>
      <div class="col">
        <a href="#">Central de Mídia</a>
        <a href="#">Termos de Uso</a>
        <a href="#">Entre em Contato</a>
      </div>
    </div>

    <button class="lang-btn">
      <i class="fa-solid fa-globe"></i> Português
      <img src="/src/assets/down-icon.png" />
    </button>

    <p class="copyright-text">Netflix Brasil</p>
  </div>
</template>


<script>
export default {
  name: 'FooterComponent',
};
</script>

<style scoped>
.footer {
  padding: 50px 15% 10px;
  border-top: 6px solid #333;
  color: #777;
}

.footer h2 {
  font-size: 18px;
  font-weight: 400;
  margin-bottom: 30px;
}

.footer .col {
  flex-basis: 25%;
  flex-grow: 1;
  margin-bottom: 20px;
}

.footer .col a {
  display: block;
  color: #777;
  font-size: 14px;
  margin-bottom: 10px;
  text-decoration: none;
}

.footer .row {
  align-items: flex-start;
  padding: 10px 0px;
}

.footer .lang-btn {
  display: inline-flex;
  align-items: center;
  gap:5px;
  background: transparent;
  border: 1px solid #fff;
  padding: 7px 10px;
  color: #FFF;
  border-radius: 3px;
}

.footer .lang-btn img {
  width: 10px;
  margin-left: 10px;
}


.copyright-text {
  font-size: 14px;
  margin-top: 20px;
  margin-bottom: 10px;
}

@media only screen and (max-width: 600px) {
  .footer .col {
    flex-basis: 100%;
  }
}
</style>
