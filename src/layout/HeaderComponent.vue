<script setup>
    import { reactive, ref } from 'vue';
    import ArrowMenu from '../components/icons/ArrowMenu.vue';

    const homePageInfo = reactive({
        href: "../App.vue",
        id: "company_name",
    });
</script>

<template>
    <header class="flex justify-between p-5">
        <a :="homePageInfo">The People</a>
        <div class="container_menu_options">
            <ArrowMenu />
        </div>
    </header>
</template>

<style scoped>
    header {
        border: 2px solid red;
    }
</style>
