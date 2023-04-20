<template>
  <div :class="bgClass">
    <div
      class="text-[#01CB63] absolute bottom-5 right-5 w-[125px] italic flex justify-center items-center bg-[#000] h-[40px] rounded-lg"
    >
      Business
    </div>
  </div>
  <div class="w-4/5 mt-5 font-bold tracking-wider text-xl mx-4">
    Ultimate Business Intelligence Analyst A to Z Course 2021
  </div>
  <div class="w-4/5 mt-5 text-sm mx-4">
    <span class="font-bold">46995</span> <span class="italic"> Student</span>
  </div>
  <div class="w-full flex justify-between">
    <div class="ml-3">1</div>
    <div class="mr-3">2</div>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  topa: String,
  bgClass: {
    type: String,
    default: "bg-yellow-300",
  },
});
</script>
