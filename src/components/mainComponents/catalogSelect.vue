<template>
    <div class="container__select">
        <div class="select__header">
            <a href="#">Главная</a>/
            <a href="#">Каталог</a>/
            <a href="#">Шины</a>
        </div>
        <hr>
        <div class="select__sort">
            Сортировать
            <button class="button" @click="isOpen = !isOpen">
                Цене
                <div class="arrow"><LogoCatalogArrow /></div>
            </button>
            <!-- <ul v-if="isOpen">
                <li>1</li>
                <li>2</li>
                <li>3</li>
            </ul> -->
            Показывать
            <button>
                Популярное
                <div class="arrow"><LogoCatalogArrow /></div>
            </button>
        </div>
    </div>
</template>

<style scoped>
.container__select {
    display: flex;
    flex-direction: column;
    margin-bottom: 30px;
}

a {
    color: rgba(0, 0, 0, 0.4);
}

p:after{
    content: '';
    display: block;
    height: 1px;
    background: #0E5FAD;
}

.select__header {
    display: flex;
    width: 250px;
    justify-content: space-between;
    color: #0E5FAD;
    margin-bottom: 13px;
}
.select__sort {
    display: flex;
    justify-content: end;
    align-items: center;
    margin-top: 33px;
}
button {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 127px;
    height: 36px;
    background-color: white;
    padding: 0 15px;
    border: 1px solid rgba(14, 95, 173, 0.1);
    color: rgba(0, 0, 0, 0.4);
    font-size: 14px;
    margin-left: 15px;
}
.button {
    margin-right: 30px;
}
.arrow {
    rotate: 90deg;
}
</style>

<script>
import LogoCatalogArrow from '@/assets/svg/LogoCatalogArrow.vue';
export default {
    name: "catalogSelect",
    data () {
        return {
            isOpen: false
        }
    },
    components: { LogoCatalogArrow }
}
</script>
