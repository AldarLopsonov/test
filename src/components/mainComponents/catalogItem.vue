<template>
    <div class="catalog__item">
        <div class="catalog__image"><img src="@/assets/images/image.png" alt=""></div>
        <div class="catalog__text">
            <div><LogoStar /><LogoStar /><LogoStar /><LogoStar /><LogoStar /></div>
            <div class="text"><span>BFGOODRICH All-Terrain T/A 245/70 R16 11/110S</span></div>
            <div class="price">11 580р.</div>
        </div>
    </div>
</template>

<script>
import LogoStar from '@/assets/svg/logoStar.vue';
export default {
    name: "catalogItem",
    components: { LogoStar }
}
</script>

<style scoped>
    .catlog__item {
        display: flex;
        flex-direction: column;
        width: 237px;
        height: 349px;
    }
    .catalog__image {
        margin:0 20px 0 10px 0;
        width:237px;
        height:220px
    }
    .catalog__text {
        display: flex;
        flex-direction: column;
        text-align: left;
        padding: 0 15px 10px 15px;
    }
    .text {
        color: black;
        margin-top: 14px;
        margin-bottom: 18px;
        font-size: 14px;
        line-height: 20px;
    }
    .price {
        color: #0E5FAD;
        font-size: 22px;
        line-height: 22px;
    }
</style>