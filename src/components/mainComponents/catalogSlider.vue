<template>
    <div class="slider">
        <hr>
        <div class="slider__text">
            <div>Всего 1 025 товаров</div>
            <div class="pagination">
                <a class="link" href="#"><i class="left"></i> </a>
                    <a href="#">1</a>
                    <a href="#">2</a>
                    <a href="#">3</a>
                    <a href="#">4</a>
                    <a href="#">5</a> 
                <a href="#"><i class="right"></i></a>
            </div>
        </div>
        <button>Следующая страница</button>
    </div>
</template>

<script>
export default {
    name: 'catalogSlider'
}
</script>

<style scoped>
.slider__text {
    display: flex;
    justify-content: space-between;
    font-size: 12px;
    margin-bottom: 30px;
    margin-top: 15px;
}
button {
    width: 263px;
    height: 54px;
    background: linear-gradient(70.67deg, #2296D7 12.76%, #0E5FAD 86.8%);
    font-size: 14px;
    line-height: 20px;
    color: white;
    margin-bottom: 90px;
}
i {
    border: solid black;
    border-width: 0 1px 1px 0;
    display: inline-block;
    padding: 2px;
}
.left {
    transform: rotate(135deg);
}

.link {
    margin: 0;
}

.right {
    transform: rotate(-45deg);
}

.pagination {
    width: 107px;
}
a {
    color: #999999;
    margin-left: 10px;
    font-size: 12px;
    line-height: 17px;
}
a:hover {
    color: #0E5FAD;
}
</style>