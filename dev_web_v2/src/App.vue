<template>
  <div id="app">
    <HeaderComponent />
    <div class="features">
      <div class="row">
        <div class="text-col">
          <h2>Desfrute na sua TV.</h2>
          <p>
            Assista em smart TVs, PlayStation, Xbox, Chromecast, Apple TV,
            players de Blu-ray e muito mais.
          </p>
        </div>
        <div class="img-col">
          <img src="./assets/feature-1.png" alt="feature-1" />
        </div>
      </div>
      <div class="row">
        <div class="img-col">
          <img src="./assets/feature-2.png" alt="feature-2" />
        </div>
        <div class="text-col">
          <h2>Baixe suas séries para assistir offline.</h2>
          <p>Salve seus favoritos facilmente e sempre tenha algo para assistir.</p>
        </div>
      </div>
      <div class="row">
        <div class="text-col">
          <h2>Assista em qualquer lugar.</h2>
          <p>
            Transmita filmes e séries ilimitados no seu celular, tablet, laptop
            e TV.
          </p>
        </div>
        <div class="img-col">
          <img src="./assets/feature-3.png" alt="feature-3" />
        </div>
      </div>
      <div class="row">
        <div class="img-col">
          <img src="./assets/feature-4.png" alt="feature-4" />
        </div>
        <div class="text-col">
          <h2>Crie perfis para crianças.</h2>
          <p>
            Envie as crianças em aventuras com seus personagens favoritos em um
            espaço feito só para elas — grátis com sua assinatura.
          </p>
        </div>
      </div>
    </div>

    <div class="faq">
      <h2>Perguntas Frequentes</h2>

      <ul class="accordion">
        <li>
          <input type="radio" name="accordion" id="first" />
          <label for="first">O que é a Netflix?</label>
          <div class="content">
            <p>
              A Netflix é um serviço de streaming que oferece uma ampla variedade de
              séries premiadas, filmes, animes, documentários e muito mais – em
              milhares de dispositivos conectados à internet.<br /><br />
              Você pode assistir o quanto quiser, quando quiser, sem uma
              única propaganda – tudo por um preço mensal acessível. Sempre há
              algo novo para descobrir, e novos filmes e séries são adicionados
              toda semana!
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="second" />
          <label for="second">Quanto custa a Netflix?</label>
          <div class="content">
            <p>
              Assista à Netflix no seu smartphone, tablet, Smart TV, laptop ou
              dispositivo de streaming, tudo por uma taxa mensal fixa. Os planos variam de
              R$ 19,90 a R$ 55,90 por mês. Sem custos extras, sem contratos.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="third" />
          <label for="third">Onde posso assistir?</label>
          <div class="content">
            <p>
              Assista em qualquer lugar, a qualquer hora. Faça login com sua conta Netflix para
              assistir instantaneamente na web em netflix.com no seu computador pessoal ou em qualquer
              dispositivo conectado à internet que ofereça o aplicativo Netflix, incluindo smart TVs, smartphones, tablets,
              players de mídia de streaming e consoles de jogos.<br /><br />
              Você também pode baixar suas séries favoritas com o aplicativo iOS, Android ou
              Windows 10. Use downloads para assistir enquanto estiver em movimento
              e sem uma conexão com a internet. Leve a Netflix com você
              para qualquer lugar.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="fourth" />
          <label for="fourth">Como faço para cancelar?</label>
          <div class="content">
            <p>
              A Netflix é flexível. Não há contratos complicados e nem
              compromissos. Você pode cancelar sua conta online facilmente em dois
              cliques. Não há taxas de cancelamento – inicie ou interrompa sua
              conta a qualquer momento.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="fifth" />
          <label for="fifth">O que posso assistir na Netflix?</label>
          <div class="content">
            <p>
              A Netflix tem uma vasta biblioteca de longas-metragens, documentários,
              séries, animes, originais premiados da Netflix e muito mais. Assista
              o quanto quiser, quando quiser.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="sixth" />
          <label for="sixth">A Netflix é boa para crianças?</label>
          <div class="content">
            <p>
              A experiência Netflix Kids está incluída na sua assinatura para dar
              aos pais controle enquanto as crianças desfrutam de séries e filmes
              voltados para a família em seu próprio espaço.<br /><br />
              Os perfis infantis vêm com controles parentais protegidos por PIN que permitem
              restringir a classificação etária do conteúdo que as crianças podem assistir e
              bloquear títulos específicos que você não quer que as crianças vejam.
            </p>
          </div>
        </li>
      </ul>

      <small>
        Pronto para assistir? Insira seu e-mail para criar ou reiniciar sua assinatura.
      </small>

      <form action="#" class="email-signup">
        <input type="email" placeholder="Endereço de e-mail" required />
        <button type="submit">Vamos lá</button>
      </form>
    </div>
    <FooterComponent />
  </div>
</template>


<script>
import HeaderComponent from './components/HeaderComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    FooterComponent,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500;700;800&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  background-color: #000;
  color: #fff;
}

.features {
  padding: 50px 12%;
  font-size: 22px;
}

.row {
  display: flex;
  align-items: center;
  width: 100%;
  flex-wrap: wrap;
  padding: 50px 0;
}

.text-col,
.img-col {
  flex-basis: 50%;
  margin-bottom: 20px;
}

.img-col img {
  display: block;
  width: 90%;
  margin: auto;
}

.features h2 {
  font-size: 50px;
  font-weight: 600;
  margin-bottom: 20px;
}

.faq {
  padding: 10px 12%;
  text-align: center;
  font-size: 18px;
}

.faq h2 {
  font-size: 40px;
  font-weight: 500;
}

.accordion {
  margin: 60px auto;
  width: 100%;
  max-width: 750px;
}

.accordion li {
  list-style: none;
  width: 100%;
  padding: 5px;
}

.accordion li label {
  display: flex;
  align-items: center;
  padding: 20px;
  font-size: 18px;
  font-weight: 500;
  background-color: #303030;
  margin-bottom: 2px;
  cursor: pointer;
  position: relative;
}

label::after {
  content: '+';
  font-size: 34px;
  position: absolute;
  right: 20px;
  transition: transform 0.5s;
}

input[type='radio'] {
  display: none;
}

.accordion .content {
  background-color: #303030;
  text-align: left;
  padding: 0 20px;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.5s, padding 0.5s;
}

.accordion input[type='radio']:checked + label + .content {
  max-height: 600px;
  padding: 30px 20px;
}

.accordion input[type='radio']:checked + label::after {
  transform: rotate(135deg);
}

.faq small {
  font-size: 13px;
}

.faq .email-signup {
  max-width: 600px;
  margin: 20px auto 60px;
}

.faq .email-signup {
    background: #fff;
    border-radius: 4px;
    display: flex;
    align-items: center;
    margin-top: 30px;
    overflow: hidden;
}

.faq .email-signup input {
    flex: 1;
    border: 0;
    outline: 0;
    margin-left: 20px;

}
.faq .email-signup button {
    background-color: #db0001;
    border: none;
    outline: none;
    color: #fff;
    font-size: 16px;
    cursor: pointer;
    padding: 15px 30px;
}

@media only screen and (max-width: 600px) {
  .text-col,
  .img-col {
    flex-basis: 100%;
  }

  .features h2 {
    font-size: 30px;
  }

  .features p {
    font-size: 15px;
  }

  .row:nth-child(2),
  .row:nth-child(4) {
    flex-direction: column-reverse;
  }

  .features .row {
    padding: 10px 0;
  }

  .faq h2 {
    font-size: 20px;
  }

  .accordion .content {
    font-size: 14px;
  }

  .accordion li label {
    padding: 10px;
    font-size: 14px;
  }

  label::after {
    font-size: 22px;
  }
  
  .faq .email-signup button {
    font-size: 12px;
    padding: 10px 15px;
  }

}
</style>
