<template>
  <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
    <div v-for="idx in list" :key="idx">
      <img
        class="
          h-full
          md:h-full
          w-full
          rounded-2xl
          cursor-pointer
          hover:shadow-xl
        "
        :src="idx"
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        "https://nogozo.com/static/book/images/sell.webp",
        "https://nogozo.com/static/book/images/neet.webp",
        "https://nogozo.com/static/book/images/all.webp",
        "https://nogozo.com/static/book/images/iit.webp",
      ],
    };
  },
};
</script>
