<template>
    <nav class="header">
        <div class="headerOne">
            <div class="container">
                <div class="about">
                    <a href="#">О компании</a>
                    <a href="#">Клиентам</a>
                    <a href="#">Для оптовиков</a>
                </div>
                <div class="dropdown">
                    <div class="menu-item"><a href="#"><DropdownCity title="Ваш город" :items="город" /> </a></div>
                    <LogoArrow />
                </div>
                <div>
                    <LogoPhone />
                    <a href="tel:8 800 2000 600" class="phone">8 800 2000 600</a></div>
                <div>
                    <LogoLock />
                    <a href="#" class="line">Войти</a>
                    <a href="#">Регистрация</a>
                </div>
            </div>
        </div>
        <div class="headerTwo"> 
            <div class="container">
                <div class="logo">
                    <a href="#"><LogoMagma /></a>
                </div>
                <div class="aboutList">
                    <a href="#">Акции</a>
                    <a href="#">Новости</a>
                    <a href="#">Услуги</a>
                    <a href="#">Контакты</a>
                </div>
                <div class="shop">
                    <LogoHeart />
                    <div class="shopProducts">
                        <div class="tovar">Нет товаров</div>
                        <div class="izbr">Избранное</div>
                    </div>
                    <LogoCart />
                    <div class="shopCart">
                    <div class="tovar">0.00 р.</div>
                    <div class="izbr">Корзина</div>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<style scoped>

.header {
    height: 100%;
    color: rgba(255, 255, 255, 0.8);
}

p {
    color: rgba(255, 255, 255, 0.8);
}

a:hover {
    color: #FFC808;
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.headerOne {
    background-color: #051F37;
    height: 39px;
    font-size: 14px;
    line-height: 1rem;
    color: white;
}

.about {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 326px;
    height: 100%;
}

.aboutList{
    display: flex;
    justify-content: space-between;
    width: 352px;
    font-size: 16px;
    line-height: 1rem;
}

.headerTwo {
    background-color: #0E5FAD;
    height: 112px;
    color: white;
}

.shop {
    display: flex;
    width: 250px;
    margin-top: 10px;
    text-align: left;
}

.line {
    padding-right: 9px;
    margin-right: 9px;
    border-right: 1px solid #FFFFFF;
}

.shopProducts {
    margin-right: 30px;
}

.izbr {
    font-size: 10px;
    line-height: 12px;
    color: rgba(255, 255, 255, 0.3);
}

.dropdown {
    display: flex;
    align-items: center;
    justify-content: center;
}
.menu-item {
    position: relative;
    text-align: center;
    display: flex;
    transition: 0.4s;
}

</style>


<script>
import LogoMagma from "../assets/svg/Header/LogoMagma.vue";
import LogoArrow from "../assets/svg/Header/LogoArrow.vue";
import LogoPhone from "@/assets/svg/Header/LogoPhone.vue";
import LogoLock from "../assets/svg/Header/LogoLock.vue";
import LogoHeart from "@/assets/svg/Header/LogoHeart.vue";
import LogoCart from "@/assets/svg/logoCart.vue";
import DropdownCity from "./headerComponents/dropdownCity.vue";

export default {
    name: 'TheHeader',
    data () {
        return {
            город: [
                {
                    title: 'Чита',
                    link: '#'
                },
                {
                    title: 'Улан-Удэ',
                    link: '#'
                },
                {
                    title: 'Иркутск',
                    link: '#'
                },
            ]
        }
    },
    components: {
    LogoMagma,
    LogoArrow,
    LogoPhone,
    LogoLock,
    LogoHeart,
    LogoCart,
    DropdownCity
}
}
</script>