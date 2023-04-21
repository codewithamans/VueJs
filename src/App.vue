<script setup>
import Courses from "./components/Courses.vue";
import Earners from "./components/Earners.vue";
import Main from "./components/Main.vue";
import Navbar from "./components/Navbar.vue";
import Comments from "./components/Comments.vue";
</script>

<template>
  <Navbar />
  <Main />
  <Courses />
  <Earners />
  <Comments />
</template>

<style scoped>
body {
  margin: 0;
  padding: 0;
}
</style>
