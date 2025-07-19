<script setup>
    import { reactive, ref } from 'vue';
    import ArrowMenu from '../components/icons/ArrowMenu.vue';

    const homePageInfo = reactive({
        href: "#",
        id: "company_name",
    });

    const isMenuOpen = ref(false);
    function toogleMenu () {
        isMenuOpen.value = !isMenuOpen.value;
    }

    function closeMenuAndNavigate (event) {
        isMenuOpen.value = false;
    }
</script>

<template>
    <div class="flex justify-between p-10 absolute right-0 left-0">
        <a :="homePageInfo">The People</a>
        <div class="container_menu_options">
            <ArrowMenu
                @click="toogleMenu" 
                :class="{ '-rotate-90' : isMenuOpen}"
                class="transition-transform duration-300 ease-in-out"
            />
            <ul v-if="isMenuOpen"
                class="absolute top-19 right-7 text-right">
                <li><a href="#about" @click="closeMenuAndNavigate">Why Us</a></li>
                <li><a href="#doing" @click="closeMenuAndNavigate">What We Do</a></li>
                <li><a href="#pricing" @click="closeMenuAndNavigate">Pricing</a></li>
                <li><a href="#contact" @click="closeMenuAndNavigate">Contact</a></li>
            </ul>
        </div>
    </div>
</template>