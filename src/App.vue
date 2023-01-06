<script setup lang="ts">
import { RouterView } from "vue-router";
import NavbarVue from "./components/NavbarVue.vue";
</script>

<template>
  <NavbarVue></NavbarVue>
  <div class="w-[calc(100wh-20px)] min-h-[calc(100vh-70px-45px-20px)] flex">
    <RouterView></RouterView>
  </div>
  <div
    class="w-[calc(100wh-20px)] flex items-center justify-center text-center"
  >
    <p class="text-white font-semibold">&copy; Kleinz</p>
  </div>
</template>
