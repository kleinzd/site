<script setup lang="ts">
import img from "../assets/nijika.jpg";
import { onMounted, ref } from "vue";
const loadTransitionDone = ref(false);

onMounted(() => {
  setTimeout(() => {
    loadTransitionDone.value = true;
  }, 500);
});
</script>
<template>
  <div class="m-auto p-5 flex-grow">
    <div
      class="flex flex-row justify-center items-center gap-5 flex-wrap z-0 transition duration-700"
      v-bind:class="{
        '-rotate-6 opacity-0 -translate-y-[600px]': !loadTransitionDone,
      }"
    >
      <img
        :src="img"
        width="300"
        height="300"
        class="rounded-full shadow-lg transition hover:rotate-6"
      />
      <div class="flex flex-col gap-2">
        <h1 class="text-5xl font-bold text-white -rotate-2">Kleinz</h1>
        <p class="text-lg font-semibold text-white">
          Hi! I'm Kleinz! 14 year old student and hobbyist developer
        </p>
        <div class="flex flex-row gap-2 flex-wrap">
          <a href="https://twitter.com/kleinztwt">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 3333 3333"
              shape-rendering="geometricPrecision"
              text-rendering="geometricPrecision"
              image-rendering="optimizeQuality"
              fill-rule="evenodd"
              clip-rule="evenodd"
              class="w-[35px] h-[35px] transition hover:scale-110 hover:rotate-12"
            >
              <path
                d="M1667 0c460 0 877 187 1179 488 302 302 488 718 488 1179 0 460-187 877-488 1179-302 302-718 488-1179 488-460 0-877-187-1179-488C186 2544 0 2128 0 1667c0-460 187-877 488-1179C790 186 1206 0 1667 0zm867 1129c-64 29-132 47-204 56 74-44 130-114 157-197-69 41-145 70-226 86-65-69-157-112-260-112-197 0-356 159-356 356 0 28 3 55 9 81-296-15-558-157-733-372-31 54-48 116-48 179 0 123 63 232 158 296-58-2-113-18-161-44v4c0 172 123 316 286 349-30 8-61 13-94 13-23 0-45-2-67-6 46 141 177 244 332 247-122 96-275 152-442 152-29 0-57-2-85-5 158 101 345 160 546 160 654 0 1013-542 1013-1013 0-16 0-31-1-46 70-50 130-112 177-184zm226-555c-280-280-666-453-1093-453S853 294 574 574c-280 280-453 666-453 1093s173 814 453 1093c280 280 666 453 1093 453s814-173 1093-453c280-280 453-666 453-1093s-173-814-453-1093z"
                fill-rule="nonzero"
                class="fill-white"
              />
            </svg>
          </a>
          <a href="https://github.com/kleinzd">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              shape-rendering="geometricPrecision"
              text-rendering="geometricPrecision"
              image-rendering="optimizeQuality"
              fill-rule="evenodd"
              clip-rule="evenodd"
              viewBox="0 0 640 640"
              class="w-[35px] h-[35px] transition hover:scale-110 hover:rotate-12"
            >
              <path
                d="M319.988 7.973C143.293 7.973 0 151.242 0 327.96c0 141.392 91.678 261.298 218.826 303.63 16.004 2.964 21.886-6.957 21.886-15.414 0-7.63-.319-32.835-.449-59.552-89.032 19.359-107.8-37.772-107.8-37.772-14.552-36.993-35.529-46.831-35.529-46.831-29.032-19.879 2.209-19.442 2.209-19.442 32.126 2.245 49.04 32.954 49.04 32.954 28.56 48.922 74.883 34.76 93.131 26.598 2.882-20.681 11.15-34.807 20.315-42.803-71.08-8.067-145.797-35.516-145.797-158.14 0-34.926 12.52-63.485 32.965-85.88-3.33-8.078-14.291-40.606 3.083-84.674 0 0 26.87-8.61 88.029 32.8 25.512-7.075 52.878-10.642 80.056-10.76 27.2.118 54.614 3.673 80.162 10.76 61.076-41.386 87.922-32.8 87.922-32.8 17.398 44.08 6.485 76.631 3.154 84.675 20.516 22.394 32.93 50.953 32.93 85.879 0 122.907-74.883 149.93-146.117 157.856 11.481 9.921 21.733 29.398 21.733 59.233 0 42.792-.366 77.28-.366 87.804 0 8.516 5.764 18.473 21.992 15.354 127.076-42.354 218.637-162.274 218.637-303.582 0-176.695-143.269-319.988-320-319.988l-.023.107z"
                class="fill-white"
              />
            </svg>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
