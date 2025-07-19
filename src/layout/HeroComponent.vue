<script setup>
    import { reactive, ref } from 'vue';

    function scrollToFirstSection () {
        const aboutSection = document.getElementById('about');
        if (aboutSection) {
            aboutSection.scrollIntoView({
                behavior: 'smooth',
                block: 'start',
            });
        }
    }
</script>

<template>
    <div id="container_general" class="min-h-dvh m-auto flex flex-col justify-center items-center">
        <div id="container_texts">
            <p class="text-3xl text-center font-bold">The People</p>
            <p class="text-base text-center m-2">To The People. <br>For The People.</p>
        </div>
        <button
            @click="scrollToFirstSection" 
            class="border-1 border-black bg-black cursor-pointer absolute bottom-12 p-2 text-gray-200 hover:bg-gray-200 hover:text-black transition-colors duration-500">
            Explore The People
        </button>
    </div>
</template>