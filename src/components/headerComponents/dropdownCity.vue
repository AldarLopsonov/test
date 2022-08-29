<template>
    <div class="menu-item" @click="isOpen = !isOpen">
        <a href="#">
            {{ title }}
        </a>
        <transition name="fade" appear>
            <div class="sub-menu" v-if="isOpen">
                <div v-for="(item,i) in items" :key="i" class="menu-item">
                    <a :href="item.link">{{ item.title }}</a>
                </div>
            </div>
        </transition>
    </div>
</template>

<script>
export default {
    name: 'dropdownCity',
    props: ['title','items'],
    data () {
        return {
            isOpen: false
        }
    }
}
</script>

<style scoped>
    .sub-menu {
        position: absolute;
        background-color: #051F37;
        top: 27px;
        width: 79px;
    }
    .sub-menu a {
        margin-bottom: 30px;
    }
</style>