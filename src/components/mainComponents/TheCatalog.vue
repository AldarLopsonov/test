<template>
	<div class="catalog">
		<div class="catalog__wrapper">
			<button class="catalog__header" @click="isOpen = !isOpen"><span>Каталог</span><MenuBurger /></button>
			<ul class="catalog__list" v-if="isOpen">
				<li>
					<a href="#"><LogoCatalog /><div class="text">Кузовные детали</div><LogoCatalogArrow /></a>
				</li>
				<li>
					<a href="#"><LogoCatalog /><div class="text">Запчасти для ТО</div><LogoCatalogArrow /></a>
				</li>			
				<li>
					<a href="#"><LogoCatalog /><div class="text">Оптика</div><LogoCatalogArrow /></a>
				</li>			
				<li>
					<a href="#"><LogoCatalog /><div class="text">Автолампы</div><LogoCatalogArrow /></a>
				</li>			
				<li>
					<a href="#"><LogoCatalog /><div class="text">Диски и Шины</div><LogoCatalogArrow /></a>
				</li>			
				<li>
					<a href="#"><LogoCatalog /><div class="text">Аккумуляторы</div><LogoCatalogArrow /></a>
				</li>			
				<li>
					<a href="#"><LogoCatalog /><div class="text">Смазочные материалы</div><LogoCatalogArrow /></a>
				</li>			
				<li>
					<a href="#"><LogoCatalog /><div class="text">Аксессуары</div><LogoCatalogArrow /></a>
				</li>						
			</ul>
		</div>
	</div>			
</template>

<script>
import LogoCatalog from '@/assets/svg/LogoCatalog.vue';
import LogoCatalogArrow from '@/assets/svg/LogoCatalogArrow.vue';
import MenuBurger from '@/assets/svg/menuBurger.vue';
export default {
    name: "TheCatalog",
    data () {
        return {
            isOpen: false
        }
    },
    components: { LogoCatalog, LogoCatalogArrow, MenuBurger }
}
</script>

<style scoped>

.catalog {
	width: 238px;
    margin-bottom: 48px;
}
.catalog__header {
	background-color: #0E5FAD;
    height: 52px;
    width: 238px;
    font-weight: bold;
    padding: 0 15px 0 15px;
    border: 1px solid #e0e0e0;
    border-bottom: none;
    border-top: none;
    justify-content: space-between;
    align-items: center;
    display: flex;
    color: white;
}
/* .catalog__list {
    position: relative;
    z-index: 2;
} */
.text {
    width:100%;
    text-align: left;
    padding-left: 9px;
}
li {
    list-style: none;
}
a {
    height: 52px;
    font-size: 14px;
    padding: 0 15px 0 15px;
    border: 1px solid #e0e0e0;
    align-items: center;
    border-top: none;
    display: flex;
}
/* .catalog__item:hover .catalog__subcatalog { 
    opacity: 1;
    visibility: visible; 
    left: 260px; 
} */
/* .catalog__subcatalog-link {
    font-size: 14px;
    color: #111;
    padding-top: 5px;
    padding-bottom: 5px;
} */
a {
    color: #111;
    text-decoration: none;
}
a:hover {
    color: #cb2d41;
}
</style>