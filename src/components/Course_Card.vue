<template>
  <div :class="bgClass">
    <div
      class="text-[#01CB63] absolute bottom-5 right-5 w-[125px] italic flex justify-center items-center bg-[#000] h-[40px] rounded-lg"
    >
      {{ title }}
    </div>
  </div>
  <div class="w-4/5 mt-5 font-bold tracking-wider text-xl mx-4">
    {{ desc }}
  </div>
  <div class="w-4/5 mt-5 text-sm mx-4">
    <span class="font-bold">{{ student_no }}</span>
    <span class="italic"> Student</span>
  </div>
  <div class="w-full flex justify-between mt-5">
    <div class="ml-3 flex space-x-2">
      <div><img src="@/assets/images/schedule.svg" alt="" srcset="" /></div>
      <div class="italic text-[#86919D] font-semibold">{{ time }}</div>
    </div>
    <div class="mr-3 flex space-x-2">
      <div><img src="@/assets/images/time.svg" alt="" srcset="" /></div>
      <div class="italic text-[#86919D] font-semibold">
        {{ lectures }} Lectures
      </div>
    </div>
  </div>
  <hr class="w-[25rem] mt-5 ml-5 bg-[#86919D]" />
  <div class="w-full flex justify-between mt-5 mb-3">
    <div class="ml-3 flex space-x-2">
      <div>
        <img
          src="@/assets/images/woodwatch.jpg"
          class="rounded-full w-[3rem] h-[3rem]"
          alt="No image"
          srcset=""
        />
      </div>
      <div class="text-black font-bold mt-3 ml-3">{{ name }}</div>
    </div>
    <div class="mr-3 flex space-x-2">
      <div class="text-[#01CB63] font-bold mt-2 text-xl">
        &#x20B9; {{ price }}
      </div>
      <div class="text-[#86919D] text-sm mt-[14px] line-through">
        {{ price }}
      </div>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  title: String,
  desc: String,
  student_no: String,
  time: String,
  lectures: String,
  name: String,
  price: String,
  bgClass: {
    type: String,
    default: "bg-yellow-300",
  },
});
</script>
