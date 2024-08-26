<template>
  <div id="app">
    <HeaderComponent />
    <div class="features">
      <div class="row">
        <div class="text-col">
          <h2>Enjoy on your TV.</h2>
          <p>
            Watch on smart TVs, PlayStation, Xbox, Chromecast, Apple TV,
            Blu-ray players and more.
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
          <h2>Download your shows to watch offline.</h2>
          <p>Save your favourites easily and always have something to watch.</p>
        </div>
      </div>
      <div class="row">
        <div class="text-col">
          <h2>Watch everywhere.</h2>
          <p>
            Stream unlimited movies and TV shows on your phone, tablet, laptop,
            and TV.
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
          <h2>Create profiles for children.</h2>
          <p>
            Send children on adventures with their favourite characters in a
            space made just for them—free with your membership.
          </p>
        </div>
      </div>
    </div>

    <div class="faq">
      <h2>Frequently Asked Questions</h2>

      <ul class="accordion">
        <li>
          <input type="radio" name="accordion" id="first" />
          <label for="first">What is Netflix?</label>
          <div class="content">
            <p>
              Netflix is a streaming service that offers a wide variety of
              award-winning TV shows, movies, anime, documentaries and more – on
              thousands of internet-connected devices.<br /><br />
              You can watch as much as you want, whenever you want, without a
              single ad – all for one low monthly price. There's always
              something new to discover, and new TV shows and movies are added
              every week!
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="second" />
          <label for="second">How much does Netflix cost?</label>
          <div class="content">
            <p>
              Watch Netflix on your smartphone, tablet, Smart TV, laptop, or
              streaming device, all for one fixed monthly fee. Plans range from
              ₹ 149 to ₹ 649 a month. No extra costs, no contracts.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="third" />
          <label for="third">Where can I watch?</label>
          <div class="content">
            <p>
              Watch anywhere, anytime. Sign in with your Netflix account to
              watch instantly on the web at netflix.com from your personal
              computer or on any internet-connected device that offers the
              Netflix app, including smart TVs, smartphones, tablets, streaming
              media players and game consoles.<br /><br />
              You can also download your favourite shows with the iOS, Android,
              or Windows 10 app. Use downloads to watch while you're on the go
              and without an internet connection. Take Netflix with you
              anywhere.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="fourth" />
          <label for="fourth">How do I cancel?</label>
          <div class="content">
            <p>
              Netflix is flexible. There are no annoying contracts and no
              commitments. You can easily cancel your account online in two
              clicks. There are no cancellation fees – start or stop your
              account anytime.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="fifth" />
          <label for="fifth">What can I watch on Netflix?</label>
          <div class="content">
            <p>
              Netflix has an extensive library of feature films, documentaries,
              TV shows, anime, award-winning Netflix originals, and more. Watch
              as much as you want, anytime you want.
            </p>
          </div>
        </li>
        <li>
          <input type="radio" name="accordion" id="sixth" />
          <label for="sixth">Is Netflix good for Kids?</label>
          <div class="content">
            <p>
              The Netflix Kids experience is included in your membership to give
              parents control while kids enjoy family-friendly TV shows and
              films in their own space.<br /><br />
              Kids profiles come with PIN-protected parental controls that let
              you restrict the maturity rating of content kids can watch and
              block specific titles you don’t want kids to see.
            </p>
          </div>
        </li>
      </ul>

      <small>
        Ready to watch? Enter your email to create or restart your membership.
      </small>

      <form action="#" class="email-signup">
        <input type="email" placeholder="Email address" required />
        <button type="submit">Get Started</button>
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
