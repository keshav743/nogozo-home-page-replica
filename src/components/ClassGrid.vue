<template>
  <div class="grid grid-cols-2 lg:grid-cols-10 gap-2">
    <div v-for="cls in classes" :key="cls" class="flex flex-col">
      <div
        class="
          text-center
          shadow-sm
          bg-blue-300
          hover:bg-blue-400 hover:shadow-md
          p-5
          rounded-xl
          cursor-pointer
          mx-1
        "
      >
        <p class="text-xl text-blue-900 font-bold">{{ cls.class }}</p>
      </div>
      <div class="text-center">
        <p>{{ cls.sub }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      classes: [
        { class: "9", sub: "Class 9" },
        { class: "10", sub: "Class 10" },
        { class: "11", sub: "Class 11" },
        { class: "12", sub: "Class 12" },
        { class: "1-8", sub: "Class 1-8" },
        { class: "IIT", sub: "IIT JEE" },
        { class: "NEET", sub: "NEET" },
        { class: "ICSE", sub: "ICSE" },
        { class: "Govt", sub: "GOVT" },
        { class: "Engg.", sub: "ENGG" },
      ],
    };
  },
};
</script>
