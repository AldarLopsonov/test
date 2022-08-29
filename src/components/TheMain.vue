<template>
    <div class="container">
        <div class="catalog">
            <TheCatalog />
            <CatalogFilter />
        </div>
        <div class="main_items">
            <InputMain />
            <CatalogSelect />
            <CatalogContent />
            <CatalogSlider />
        </div>
    </div>
</template>

<style scoped>
    .container {
        display: flex;
        flex-direction: row;
        margin-top: 30px;
    }
    .catalog {
    }
    .main_items {
        display: flex;
        flex-direction: column;
        margin-left: 30px;
        color:rgba(0, 0, 0, 0.4);
    }
</style>

<script>
import TheCatalog from "../components/mainComponents/TheCatalog.vue";
import InputMain from "./mainComponents/InputMain.vue";
import CatalogContent from "./mainComponents/catalogContent.vue";
import CatalogSelect from "./mainComponents/catalogSelect.vue";
import CatalogSlider from "./mainComponents/catalogSlider.vue";
import CatalogFilter from "./mainComponents/catalogFilter.vue";
export default {
    name: 'TheMain',
    components: {
    TheCatalog,
    InputMain,
    CatalogContent,
    CatalogSelect,
    CatalogSlider,
    CatalogFilter
}
}
</script>