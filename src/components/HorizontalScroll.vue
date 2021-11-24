<template>
  <div class="grid grid-cols-2 lg:grid-cols-6 gap-6">
    <div
      v-for="item in items"
      :key="item.id"
      class="shadow-sm hover:shadow-lg rounded-xl cursor-pointer"
    >
      <div class="flex flex-col p-10 bg-gray-100 rounded-t-xl">
        <img :src="item.image" />
      </div>
      <div class="p-2">
        <p class="font-bold text-gray-800">{{ item.name }}</p>
        <p class="font-normal text-gray-500 text-sm">By {{ item.author }}</p>
        <p>
          <span class="text-blue-500 font-semibold text-sm"
            >Rs. {{ item.discountPrice }}</span
          >
          <span class="ml-2 text-gray-500 font-semibold text-sm"
            ><s>Rs. {{ item.price }}</s></span
          >
        </p>
        <p class="text-green-500 font-semibold text-sm">
          {{ item.discount }} off
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["items"],
};
</script>
