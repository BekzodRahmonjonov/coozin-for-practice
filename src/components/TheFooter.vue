<template>
    <footer>
        <div class="container">
            <div class="footer">
                <div class="footer__top">
                    <div class="footer__logo">
                        <img src="../assets/logo_coozin.png" alt="footer-logo">
                    </div>
                    <div class="footer__items">
                        <div class="footer__nav">
                            <a href="#" class="nav__item">Наша история</a>
                            <a href="#" class="nav__item">Присоединиться</a>
                            <a href="#" class="nav__item">Блог</a>
                        </div>
                        <div class="footer__pay">
                            <h3>Безопаская оплата</h3>
                            <div class="footer__pay-img">
                                <img src="../assets/apelsin_logo.png" alt="apelsin-logo">
                            </div>
                        </div>
                        <div class="footer__support">
                            <h3>При поддержке</h3>
                            <div class="support__images">
                                <img src="../assets/cola_logo.png" alt="cola-logo">
                                <img src="../assets/osce_logo.png" alt="osce-logo">
                            </div>
                        </div>
                    </div>
                </div>
                <div class="footer__bottom">
                    <div class="footer__lisence">© 2022 Coozin  All Rights Reserved</div>
                    <div class="footer__social">
                        <div class="social__text">
                            <p>ПОДПИСЫВАЙТЕСЬ НА НАС</p>
                            <div class="social__line"></div>
                        </div>
                        <div class="social__images">
                            <a href=""><img src="../assets/insta.png" alt="insta"></a>
                            <a href=""><img src="../assets/facebook.png" alt="facebook"></a>
                            <a href=""><img src="../assets/YT.png" alt="youtube"></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "TheFooter"
}
</script>

<style scoped>
footer{
    border: 1px solid red;
    padding: 50px 10px 30px;
}

.footer__top{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-around;
}

.footer__items{
    width: 100%;
    max-width: 724px;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.footer__logo{
    width: 148px;
}

.footer__logo>img{
    width: 100%;
}

.nav__item{
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;
    color: #242C39;
    text-decoration: none;
    display: block;
    margin-bottom: 20px;
}

.nav__item:last-child{
    margin-bottom: 0px;
}

.nav__item:hover{
    color: red;
}

h3{
    color: #374151;
    font-weight: 600;
    font-size: 16px;
    line-height: 24px;
    margin-bottom: 19px;
}

.support__images{
    display: flex;
    justify-content: space-between;
    width: 200px;
}

.footer__bottom{
    margin-top: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.footer__lisence{
    font-weight: 300;
    font-size: 16px;
    line-height: 24px;
    color: #1F2937;
}
.footer__social{
    display: flex;
    align-items: center;
}

.footer__social p{
    font-weight: 600;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: 0.1em;
    color: #1F2937;
    position: relative;
}

.social__line{
    width: 60px;
    border: 1px solid #1F2937;
    margin: 0px 10px;
}

.social__text{
    display: flex;
    align-items: center;
}
.social__images a{
    width: 35px;
    height: 35px;
    margin: 0px 5px;
}

.social__images img{
    width: 100%;
}

.social__images{
    display: flex;
    align-content: center;
}

.footer__nav , .footer__pay , .footer__support{
    margin: 0px 10px;
}

@media (max-width: 768px) {
    .footer__bottom{
        flex-direction: column-reverse;
        justify-content: space-between;
        margin-top: 30px;
    }
    .footer__lisence{
        margin-top: 5px;
    }
}
</style>
