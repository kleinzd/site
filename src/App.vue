<script setup lang="ts">
import { RouterView } from "vue-router";
import NavbarVue from "./components/NavbarVue.vue";
</script>

<template>
  <NavbarVue></NavbarVue>
  <div class="bg-[#343434] w-screen min-h-[calc(100vh-70px-45px)] flex">
    <RouterView></RouterView>
  </div>
  <div
    class="w-screen h-[45px] bg-[#343434] flex items-center justify-center text-center"
  >
    <p class="text-white font-semibold">&copy; Kleinz</p>
  </div>
</template>
