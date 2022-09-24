<script setup lang="ts">
import { RouterLink } from "vue-router";
import img from "../assets/takina.png";
</script>

<template>
  <div class="bg-[#292929] w-screen h-[70px] flex items-center px-5">
    <ul class="flex flex-column gap-7 items-center">
      <li class="transition hover:translate-y-3">
        <RouterLink :to="{ name: 'Home' }"
          ><img :src="img" class="h-[55px] w-[55px] shadow-lg rounded-full"
        /></RouterLink>
      </li>
      <li class="text-white font-semibold hover:text-teal-500 transition">
        <RouterLink to="/">Home</RouterLink>
      </li>
      <li class="text-white font-semibold hover:text-teal-500 transition">
        <RouterLink to="/about">About</RouterLink>
      </li>
    </ul>
  </div>
</template>
