<template>
  <div class="w-full bg-yellow h-auto">
    <div
      class="w-full text-[#01CB63] italic text-center mt-10 md:mt-32 text-xl md:text-2xl"
    >
      Courses
    </div>
    <div class="w-full text-black text-center mt-4 text-4xl md:text-5xl">
      Our Most Popular Courses
    </div>
    <div class="flex justify-center items-center">
      <div class="w-full md:w-4/5">
        <div
          class="grid grid-cols-1 lg:grid-cols-3 gap-4 lg:gap-12 mt-8 md:mt-20"
        >
          <div class="h-auto shadow-lg shadow-gray-400 rounded-xl">
            <Course_Card
              title="Business"
              desc="Ultimate Business Intelligence Analyst A to Z Course 2021"
              student_no="46,995"
              time="11 hr 20 mins"
              lectures="44"
              img="@/assets/images/carla.jpg"
              name="Albert Hitler"
              price="2000"
              bgClass="bg-business rounded-xl w-full h-[300px] relative bg-slate-500"
            />
          </div>
          <div class="h-auto shadow-lg shadow-gray-400 rounded-xl">
            <Course_Card
              title="Design"
              desc="Adobe Photoshop Training: From Beginner to Pro"
              student_no="6,995"
              time="6 hr 20 mins"
              lectures="24"
              name="Wanda Wilson"
              price="3000"
              bgClass="bg-design rounded-xl w-full h-[300px] relative bg-slate-500"
            />
          </div>
          <div class="h-auto shadow-lg shadow-gray-400 rounded-xl">
            <Course_Card
              title="Marketing"
              desc="Social Media Marketing - A to Z Content Marketing class 2021"
              student_no="46,995"
              time="11 hr 20 mins"
              lectures="44"
              name="Albert Hitler"
              price="2000"
              bgClass="bg-marketing rounded-xl w-full h-[300px] relative bg-slate-500"
            />
          </div>
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
