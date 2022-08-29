<template>
    <ul>
        <li><a href="#">Оплата</a></li>
        <li><a href="#">Доставка</a></li>
        <li><a href="#">Возврат</a></li>
        <li><a href="#">СТО</a></li>
        <li><a href="#">Шинные центры</a></li>
        <li><a href="#">АЗС Авангард-75</a></li>
        <li><a href="#">Бонусная программа</a></li>
    </ul>
</template>

<script>
export default {
    name: 'footerLinks'
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
    text-align: start;
}
a:hover {
    color: white;
}

</style>