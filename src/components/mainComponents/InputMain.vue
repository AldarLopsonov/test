<template>
    <div class="input__container">
        <div class="search__list">
            <button class="search__button" @click="isOpen = !isOpen">
                По артикулу
                <div class="arrow"><LogoCatalogArrow /></div>
            </button>
            <ul v-if="isOpen">
                <li class="list"><a href="#">По чему-то еще</a></li>
                <li class="list"><a href="#">По чему-то еще</a></li>
                <li class="list"><a href="#">По чему-то еще</a></li>
            </ul>
        </div>
        <input type="text" placeholder="Поиск по сайту">
        <div class="search__icon">
            <LogoSearch />
        </div>
    </div>
</template>

<script>
import LogoSearch from '@/assets/svg/logoSearch.vue';
import LogoCatalogArrow from '@/assets/svg/LogoCatalogArrow.vue';
export default {
    name: "InputMain",
    data () {
        return {
            isOpen: false
        }
    },
    components: { LogoSearch, LogoCatalogArrow}
}
</script>

<style scoped>
.input__container {
    display: flex;
    width: 772px;
    height: 52px;
    /* border: 1px solid #0E5FAD; */
    margin-bottom: 30px;
    z-index: 1;
}
.search__list {
    width: 162px;
}
.search__button {
    display: flex;
    justify-content: space-between;
    width: 162px;
    height: 52px;
    background-color: white;
    border: none;
    padding: 10px 15px;
    align-items: center;
    color: rgba(0, 0, 0, 0.4);
    font-size: 14px;
    border: 1px solid #0E5FAD;
}
svg {
    fill: black;
}
input {
    width: 550px;
    border: none;
    padding-left: 14px;
    border: 1px solid #0E5FAD;
    border-left: none;
}
input::-webkit-input-placeholder { color:  rgba(0, 0, 0, 0.4); }

.search__icon {
    width: 59px;
    background-color: #0E5FAD;
    display: flex;
    justify-content: center;
    align-items: center;
}
.arrow {
    rotate: 90deg;
}
ul {
    list-style: none;
}

a {
    color: rgba(0, 0, 0, 0.4);
}

.list {
    height: 52px;
    border: 1px solid #0E5FAD;
    z-index: 1;
    background-color: white;
    border-top: none;
    padding-left: 15px;
    font-size: 14px;
    text-align: left;
    display: flex;
    align-items: center;
}
</style>