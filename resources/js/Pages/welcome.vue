<script setup>
 import navigation from "../components/navigation.vue";
 import about from "../components/about.vue";
 import projects from "../components/projects.vue";
 import CustomSection from "../components/CustomSection.vue";
 defineOptions({layout: navigation})
</script>

<template>
    <transition appear name="fade">
        <CustomSection id="home">
            <div class="flex container content-center">
                <div class="flex flex-col justify-center">
                    <span class="text-4xl tracking-wider leading-loose">
                        I'm
                        <span class="text-blue-400">Lirys Nhoj Roben S. Belleza</span>
                    </span>
                    <p class="text-2xl tracking-wider">An aspiring software engineer</p>
                </div>
                <div class="flex items-center ml-auto mr-auto">
                    <img src="../../../public/test.jpg" alt=""
                         class="rounded-full h-64 w-64">
                </div>
            </div>
        </CustomSection>
    </transition>
    <CustomSection id="about" class="mt-96">
        <about/>
    </CustomSection>
    <CustomSection id="projects" class="mt-96">
        <projects/>
    </CustomSection>
</template>

<style scoped>
.fade-enter-active,
.fade-leave-active{
    transition: all 1s ease;
}

.fade-enter-from,
.fade-leave-to{
    margin-left: -100px;
    opacity: 0;
}
</style>
