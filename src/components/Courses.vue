<template>
  <div class="w-full bg-yellow h-auto">
    <div class="w-full text-[#01CB63] italic text-center mt-32 text-2xl">
      Courses
    </div>
    <div class="w-full text-black text-center mt-4 text-4xl">
      Our Most Popular Courses
    </div>
    <div class="flex justify-center items-center">
      <div class="w-4/5 bg-red-300">
        <div class="grid lg:grid-cols-3 gap-24">
          <div class="bg-yellow-300 h-[500px]">
            <Course_Card
              topa="topa"
              bgClass="bg-girl w-full h-[300px] relative bg-slate-500"
            />
          </div>
          <div class="bg-yellow-300">2</div>
          <div>3</div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Course_Card from "./Course_Card.vue";
export default {
  components: { Course_Card },
};
</script>
