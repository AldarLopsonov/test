<template>
    <div class="filter">
        <div class="filter__price">
            <div class="text">Цена</div>
            <div class="price_ammount">
                <div class="price">10 000р.</div> 
                <div class="price">90 000р.</div>
            </div>
            <input type="range" min="1" max="100" value="50" class="slider" id="myRange">
        </div>
        <FilterItem />
        <FilterItem />
        <FilterItem />
    </div>
</template>

<script>
import FilterItem from './filterItem.vue';
export default {
    name: "catalogFilter",
    components: { FilterItem }
}
</script>

<style scoped>
.filter {
    display: flex;
    flex-direction: column;
    color: #0E5FAD;
}
.filter__price {
    display: block;
    margin-bottom: 36px;
}
.text {
    text-align: left;
    font-size: 24px;
    line-height: 24px;
    margin-bottom: 8px;
}
.price_ammount{
    display: flex;
    justify-content: space-between;
    margin-bottom: 12px;
}
.price {
    border: 1px solid #ECECEC;
    border-radius: 2px;
    padding: 8px 28px;
    font-size: 12px;
    line-height: 15px;
    letter-spacing: 0.5px;
    color: black;
}
.slider {
    width: 100%;
    height: 5px;
    background:#ECECEC;
}
input {
    margin: 0;
    padding: 0;
}
</style>