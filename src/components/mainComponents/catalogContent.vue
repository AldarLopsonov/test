<template>
    <div class="catalog">
        <a href="#"><div class="catalog__item"><div class="snow"><LogoSnow /></div><CatalogItem /></div></a>
        <a href="#"><CatalogItem /></a>
        <a href="#"><div class="catalog__item"><div class="new"><TextNEW /></div><CatalogItem /></div></a>
        <a href="#"><div class="catalog__item"><div class="snow"><LogoSnow /></div><CatalogItem /></div></a>
        <a href="#"><CatalogItem /></a>
        <a href="#"><div class="catalog__item"><div class="new"><TextNEW /></div><CatalogItem /></div></a>
        <a href="#"><div class="catalog__item"><div class="snow"><LogoSnow /></div><CatalogItem /></div></a>
        <a href="#"><CatalogItem /></a>
        <a href="#"><div class="catalog__item"><div class="new"><TextNEW /></div><CatalogItem /></div></a>
        <a href="#"><div class="catalog__item"><div class="snow"><LogoSnow /></div><CatalogItem /></div></a>
        <a href="#"><CatalogItem /></a>
        <a href="#"><div class="catalog__item"><div class="new"><TextNEW /></div><CatalogItem /></div></a>
        <a href="#"><div class="catalog__item"><div class="snow"><LogoSnow /></div><CatalogItem /></div></a>
        <a href="#"><CatalogItem /></a>
        <a href="#"><div class="catalog__item"><div class="new"><TextNEW /></div><CatalogItem /></div></a>
    </div>
</template>

<style scoped>
.catalog {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: 350px;
    margin-bottom: 46px;
}
a :hover {
    color: blue;
    cursor: pointer;
}
.catalog__item {
    position: relative;
}
.snow {
    position: absolute;
    left:  20px;
}
.new {
    position: absolute;
    right: 5px;
}
</style>

<script>
import CatalogItem from './catalogItem.vue';
import LogoSnow from '../../assets/svg/logoSnow.vue';
import TextNEW from './textNEW.vue';
export default {
    name: "catalogContent",
    components: { CatalogItem, LogoSnow, TextNEW }
}
</script>

