<template>
    <section class="h-[100vh] bg-img text-white flex justify-center">
        <div class="flex items-center flex-col space-y-[1rem] md:flex-row md:justify-center py-[13rem] md:space-x-[5rem]">
            <div class="rounded-full my-img"></div>
            <div class="md:space-y-[1rem]">
                <div class="flex items-center flex-col md:space-y-[1.2rem]">
                    <div class="text-3xl md:text-[3.5rem]">Christian Gilbert Salas</div>
                    <div class="text-xl md:text-[2rem] md:bg-white md:text-black md:p-[0.2rem] md:px-[0.5rem] md:rounded-lg md:font-bold">
                        Front-End Web Developer
                    </div>
                </div>
                <div class="flex flex-col md:flex-row md:justify-center md:space-x-[2.5rem] items-center">
                    <div class="flex flex-row py-[2rem] space-x-[1rem]">
                        <NuxtLink to="https://www.facebook.com/gilbeeeerrrrtttt/"><div class="facebook-icon"></div></NuxtLink>
                        <div class="insta-icon"></div>
                        <div class="gmail-icon"></div>
                        <NuxtLink to="https://github.com/gilbert1220"><div class="github-icon"></div></NuxtLink>
                    </div>
                    <div>
                        <NuxtLink to="#about">
                            <button class="bg-white text-black flex flex-row items-center gap-2 px-[2rem] rounded-lg">
                                Get Started <p class="text-3xl"></p>
                            </button>
                        </NuxtLink>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
