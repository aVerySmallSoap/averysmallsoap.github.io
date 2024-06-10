<script setup>
import { Link } from "@inertiajs/vue3";
</script>

<template>
    <main class="border-b-gray-300 border-b shadow-lg">
        <header class="flex flex-wrap">
            <div class="flex basis-full p-2">
                <h3 class="ml-5 flex flex-wrap content-center justify-center">Belleza</h3>
                <div class="links flex ml-auto mr-5 gap-10 content-center justify-center">
                    <a class="hover:-translate-y-0.5 transition-all hover:bg-blue-400 p-1 rounded" href="#home">Home</a>
                    <a class="hover:-translate-y-0.5 transition-all hover:bg-blue-400 p-1 rounded" href="#projects">Projects</a>
                    <a  class="hover:-translate-y-0.5 transition-all hover:bg-blue-400 p-1 rounded" href="#about">About Me</a>
                </div>
            </div>
        </header>
    </main>
    <article>
        <slot/>
    </article>
</template>

<style scoped>
</style>
