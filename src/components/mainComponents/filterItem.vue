<template>
    <div class="filterItem">
        <div class="header">
            <div class="name">Фильтр</div>
            <div class="all">Все</div>
        </div>
        <hr>
        <div class="list">
            <ul class="list__wrapper">
                <li><input type="checkbox"><span>Фильтр 1</span></li>
                <li><input type="checkbox"><span>Фильтр 2</span></li>
                <li><input type="checkbox"><span>Фильтр 3</span></li>
                <li><input type="checkbox"><span>Фильтр 4</span></li>
                <li><input type="checkbox"><span>Фильтр 5</span></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'filterItem'
}
</script>

<style scoped>

.header {
    display: flex;
    justify-content: space-between;
}
.name {
    font-size: 24px;
    line-height: 24px;
    color: #0E5FAD;
}
.all {
    font-size: 12px;
    line-height: 12px;
    color: #999999;
    padding-top: 12px;
}
hr {
    background: #3A405B;
    mix-blend-mode: normal;
    opacity: 0.05;
    margin-top: 8px;
    margin-bottom: 13px;
}
ul {
    list-style: none;
    margin: 0;
    padding: 0;
    text-align: left;
}
li {
    height: 20px;
    display: flex;
    align-items: center;
    margin-bottom: 16px;
}
input {
    width: 20px;
    height: 20px;
    border: 2px solid #E4E8F0;
    border-radius: 4px;
    margin: 0;
    padding: 0;
}
span {
    font-size: 14px;
    margin-left: 13px;
    color: #3A405B;;
}
</style>