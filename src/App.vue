<script setup>
import Courses from "./components/Courses.vue";
import Earners from "./components/Earners.vue";
import Main from "./components/Main.vue";
import Navbar from "./components/Navbar.vue";
</script>

<template>
  <Navbar />
  <Main />
  <Courses />
  <Earners />
</template>

<style scoped>
body {
  margin: 0;
  padding: 0;
}
</style>
