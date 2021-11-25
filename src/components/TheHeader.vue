<template>
  <div class="flex flex-row justify-between p-3 bg-white">
    <div v-on="pressed">
      <svg
        class="w-10 h-10 md:w-12 md:h-12 rounded-full hover:bg-gray-100 p-2"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16M4 18h16"
        ></path>
      </svg>
    </div>
    <img
      class="w-20 h-8 md:w-32 md:h-12"
      src="https://nogozo.com/static/mainapp/img/logo.png"
      alt="Nogozo-alt-pic"
    />
    <svg
      class="w-10 h-10 md:w-12 md:h-12 rounded-full hover:bg-gray-100 p-2"
      fill="none"
      stroke="currentColor"
      viewBox="0 0 24 24"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
      ></path>
    </svg>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuPressed: false,
    };
  },
  methods: {
    pressed() {
      this.menuPressed = !this.menuPressed;
    },
  },
};
</script>
