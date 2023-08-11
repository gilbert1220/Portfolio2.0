<template>
    <headerNav />
    <home id="home">
        <div class="container bg-white bg-opacity-40 flex justify-center items-center max-w-[100%] z-100" id="container" :style="{ display: containerDisplay }">
            <div class="flex justify-center items-center flex-col absolute bg-black h-[15rem] w-[30rem] rounded-lg bg-opacity-50 space-y-[3rem]">
                <div class="text-3xl">Hi! Welcome to my Portfolio</div>
                <div>
                    <button @click="hideContainer" id="contiue" class="bg-black tex-white px-[2rem] rounded-lg">Continue</button>
                </div>
            </div>
        </div>
    </home>
    <about id="about" />
    <skills id="skills" />
</template>

<script>
    export default {
         data() {
        return {
        containerDisplay: "display" // Set the initial display value
        };
    },
     methods: {
    hideContainer() {
      this.containerDisplay = "none";
    }
  }
    };
</script>

<style>
    .container{
        position: fixed;
        height: 100%;
        width: 100%;
    }
</style>