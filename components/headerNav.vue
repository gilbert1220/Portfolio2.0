<script setup>
     function openNav(){
         document.querySelector('.sidebar').classList
         .toggle('left-[-15rem]');
     }
     function closeNav(){
         document.querySelector('.sidebar').classList
         .toggle('left-[-15rem]');
     }
 </script>
<template>
    <div class="w-full h-[4rem] bg-gray-900 bg-opacity-30 fixed">
        <div class="hidden md:block text-white lg:flex justify-between items-center h-full mx-[5rem]">
                <NuxtLink to="/"><div>My Logo</div></NuxtLink>
                <div class="flex flex-row space-x-[7rem]">
                    <NuxtLink to="#about"><div>About</div></NuxtLink>
                    <NuxtLink to="#skills"><div>Skills</div></NuxtLink>
                    <NuxtLink to="#"><div>Contact Me</div></NuxtLink>
                </div>
        </div>
        <div class="flex justify-between items-center h-full mx-[2rem] md:hidden">
            <div>
                <span @click="openNav" class="cursor-pointer">
                    <div class="burger"></div>
                </span>
            </div>
            <div>
                <NuxtLink to="#home">
                    <div class="">my logo</div>
                </NuxtLink>
            </div>
        </div>
    </div>
    <div class="sidebar fixed top-0 bottom-0 lg:left-0 p-2 w-[15rem] overflow-y-auto bg-gray-900 left-[-15rem] md:hidden">
        <span class="flex justify-end cursor-pointer" @click="closeNav">
            <div class="px-2 x-icon md:hidden w-fit"></div>
        </span>
        <div class="flex flex-col text-white space-y-[1rem]">
            <NuxtLink to="#home"><div>Home</div></NuxtLink>
            <NuxtLink to="#about"><div>About</div></NuxtLink>
            <NuxtLink to="#skills"><div>Skills</div></NuxtLink>
            <NuxtLink><div>Contact Me</div></NuxtLink>
        </div>
    </div>
    <slot />
</template>

