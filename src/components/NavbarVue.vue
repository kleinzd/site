<script setup lang="ts">
import { RouterLink } from "vue-router";
import img from "../assets/nijika.jpg";
</script>

<template>
  <div
    class="bg-[#51E1ED] w-[calc(100wh-20px)] h-[calc(70px)] flex items-center px-3 rounded-3xl shadow-lg z-10"
  >
    <ul class="flex flex-column gap-7 items-center">
      <li class="transition hover:translate-y-3">
        <RouterLink :to="{ name: 'Home' }"
          ><img :src="img" class="h-[55px] w-[55px] shadow-lg rounded-full"
        /></RouterLink>
      </li>
      <li class="text-[#03203C] font-semibold hover:text-[#207398] transition">
        <RouterLink to="/">Home</RouterLink>
      </li>
      <li class="text-[#03203C] font-semibold hover:text-[#207398] transition">
        <RouterLink to="/about">About</RouterLink>
      </li>
    </ul>
  </div>
</template>
