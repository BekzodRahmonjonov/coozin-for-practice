<template>
  <footer>
    <div class="container">
      <div class="footer">
        <div class="footer__menu">
          <div class="footer__menu-logo">
            <a href="/App.vue"><img src="../assets/icons/logo_coozin.svg" alt="coozin logo" /></a>
          </div>
          <div class="footer__menu-items">
            <ul class="footer__menu-nav">
              <li><a href="#">Наша история</a></li>
              <li><a href="#">Присоединиться</a></li>
              <li><a href="#">Блог</a></li>
            </ul>
            <div class="footer__payment gap">
              <h3>Безопаская оплата</h3>
              <div class="footer__payment-img">
                <img src="../assets/icons/apelsin_logo.svg" alt="apelsin logo" />
              </div>
            </div>
            <div class="footer__support gap">
              <h3>При поддержке</h3>
              <div class="footer__support-img">
                <img src="../assets/icons/cola.svg" alt="cola logo" />
                <img src="../assets/icons/osce.svg" alt="osce logo" />
              </div>
            </div>
          </div>
        </div>
        <div class="footer__contact">
          <h3 class="footer__contact-h3">© 2022 Coozin All Rights Reserved</h3>
          <div class="footer__social">
            <div class="footer__social-text">
              <p>ПОДПИСЫВАЙТЕСЬ НА НАС</p>
              <div class="footer__social-line"></div>
            </div>
            <div class="footer__social-img">
              <a href=""><img src="../assets/icons/insta.svg" alt="insta" /></a>
              <a href=""><img src="../assets/icons/facebook.svg" alt="facebook" /></a>
              <a href=""><img src="../assets/icons/yt.svg" alt="youtube" /></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter",
};
</script>

<style scoped>
footer {
  padding: 50px 10px 30px;
}

.footer__menu {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-around;
  gap: 20px;
}

.footer__menu-items {
  width: 100%;
  max-width: 724px;
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 20px;
}

.footer__menu-logo {
  width: 148px;
}

.footer__menu-logo img , .footer__menu-logo a{
  width: 100%;
}

.footer__menu-nav{
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.footer__menu-nav a{
  text-decoration: none;
  color: #242c39;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
}

.footer__menu-nav a:hover {
  color: red;
}

h3 {
  color: #374151;
  font-weight: 600;
  font-size: 16px;
  line-height: 24px;
}

.gap{
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.footer__support-img {
  display: flex;
  gap: 30px;
}

.footer__contact {
  margin-top: 100px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.footer__contact-h3 {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  color: #1f2937;
}
.footer__social {
  display: flex;
  align-items: center;
}

.footer__social p {
  font-weight: 600;
  font-size: 14px;
  line-height: 20px;
  letter-spacing: 0.1em;
  color: #1f2937;
  position: relative;
}

.footer__social-line {
  width: 60px;
  border: 1px solid #1f2937;
  margin: 0px 10px;
}

.footer__social-text {
  display: flex;
  align-items: center;
}
.footer__social-img a {
  width: 35px;
  height: 35px;
  margin: 0px 5px;
}

.footer__social-img img {
  width: 100%;
}

.footer__social-img {
  display: flex;
  align-content: center;
}

li{
  list-style: none;
}

@media (max-width: 768px) {
  .footer__contact {
    flex-direction: column-reverse;
    justify-content: space-between;
    margin-top: 30px;
  }
  .footer__contact-h3 {
    margin-top: 5px;
  }
}
@media (max-width: 480px) {
  .footer__social-text{
    display: none;
  }
  .footer__social-img{
    gap: 30px;
  }
}
</style>
