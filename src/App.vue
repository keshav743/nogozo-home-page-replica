<template>
  <div class="flex flex-col">
    <div class="fixed w-full">
      <the-header></the-header>
    </div>
    <div class="mx-3 my-20">
      <main-content></main-content>
    </div>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import MainContent from "./components/MainContent.vue";

export default {
  components: {
    "the-header": TheHeader,
    "main-content": MainContent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
