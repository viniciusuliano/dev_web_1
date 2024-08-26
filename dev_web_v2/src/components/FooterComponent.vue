<template>
  <div class="footer">
    <h2>Questions? Call 000-000-000-0000</h2>

    <div class="row">
      <div class="col">
        <a href="#">FAQ</a>
        <a href="#">Investor Relations</a>
        <a href="#">Privacy</a>
        <a href="#">Speed Test</a>
      </div>
      <div class="col">
        <a href="#">Help Centre</a>
        <a href="#">Jobs</a>
        <a href="#">Cookie Preferences</a>
        <a href="#">Legal Notices</a>
      </div>
      <div class="col">
        <a href="#">Account</a>
        <a href="#">Ways to Watch</a>
        <a href="#">Corporate Information</a>
        <a href="#">Only on Netflix</a>
      </div>
      <div class="col">
        <a href="#">Media Centre</a>
        <a href="#">Terms of Use</a>
        <a href="#">Contact Us</a>
      </div>
    </div>

    <button class="lang-btn">
      <i class="fa-solid fa-globe"></i> English
      <img src="/src/assets/down-icon.png" />
    </button>

    <p class="copyright-text">Netflix United States</p>
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
