<template>
    <div class="footer">
        <div class="container">
            <div class="footer__container">
                <div class="footer__firstBlock">
                    <div class="footer__logo">
                        <a href="#"><LogoMagma /></a>
                    </div>
                    <div class="footer__text">
                        В интернет-магазине автотоваров МАСМА представленны все необходимые масла и смазки, расходные жидкости, автохимия, автозвук и различные аксессуары для автомобиля. Огромный каталог запчастей, шин и дисков с удобным онлайн подбором. 
                    </div>
                    <div class="footer__socials">
                        <div class="vk"><a href=""></a><VK /></div>
                        <div class="inst"><InstagramSocial /></div>
                    </div>
                </div>
                <div class="links">
                    <div class="links_header">
                        Каталог
                    </div>
                    <ul>
                        <li><a href="#">Кузовные детали</a></li>
                        <li><a href="#">Запчасти для ТО</a></li>
                        <li><a href="#">Оптика</a></li>
                        <li><a href="#">Автолампы</a></li>
                        <li><a href="#">Диски и шины</a></li>
                        <li><a href="#">Аккумуляторы</a></li>
                        <li><a href="#">Смазочные материалы</a></li>
                        <li><a href="#">Аксессуары</a></li>
                    </ul>
                </div>
                <div class="links">
                    <div class="links_header">
                        Клиентам
                    </div>
                    <footerLinks />
                </div>
                <div class="links">
                    <div class="links_header">
                        Оптовикам
                    </div>
                    <footerLinks />
                </div>
            </div>
        </div>
    </div>
    <div class="footerBottom">
        <div class="container">
                <div><a href="#">© МАСМА - автотовары онлайн. 2019</a></div>
                <div><a href="#">Политика конфиденциальности</a></div>
                <div><a href="#">Пользовательское соглашение</a></div>
        </div>
    </div>
</template>

<script>
import VK from '@/assets/svg/Footer/VK.vue';
import InstagramSocial from '../assets/svg/Footer/InstagramSocial.vue';
import LogoMagma from '@/assets/svg/Header/LogoMagma.vue';
import footerLinks from './footerComponents/footerLinks.vue';
    export default {
    name: 'TheFooter',
    components: {
    VK,
    InstagramSocial,
    LogoMagma,
    footerLinks,
}
}
</script>

<style scoped>

ul {
    padding: 0;
    margin: 0;
}
li {
    list-style: none;
    margin: 0;
    padding: 0;
}
a {
    font-size: 14px;
    line-height: 22px;
    color: rgba(255, 255, 255, 0.5);;
}

a:hover {
    color: white;
}

.footer {
    display: flex;
    background-color: #051F37;
    height: 457px;
}

.footer__container {
    display: flex;
    justify-content: space-between;
    margin: 70px 0 60px 0;
    width: 1040px;
}

.footer__logo {
    margin-bottom: 25px;
}

.footer__text {
    font-size: 14px;
    line-height: 22px;
    color: rgba(255, 255, 255, 0.5);;
    text-align: start;
    margin-bottom: 20px;
}

.footer__socials {
    margin-bottom: 60px;
    display: flex;
}

.vk {
    margin-right: 20px;
}
.footer__firstBlock {
    display: flex;
    flex-direction: column;
    width: 242px;
    text-align: left;
    
}

.footerBottom {
    background-color:#041729;
    height: 41px;
}

.links {
    width: 150px;
    text-align: start;
    line-height: 28px;
}
.links_header {
    margin-bottom: 20px;
}
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>