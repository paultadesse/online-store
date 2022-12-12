<template>
  <div class="group">
    <img :src="activeOption.imgPath" alt="" />
    <div class="relative">
      <div class="absolute inset-0 py-2 gap-2 hidden group-hover:block">
        <div class="gap-2 flex">
          <div v-for="(option, index) in item.options" :key="option.id">
            <img
              class="h-12 w-12"
              :src="option.imgPath"
              alt=""
              @mouseenter="activeOptionIndex = index"
            />
          </div>
        </div>
        <div class="space-y-1 py-2">
          <p class="">
            {{ activeOption.price }}
            <span class="text-gray-500 line-through px-1">$100</span>
          </p>
          <p class="py-2 text-green-600">14 % off</p>
        </div>
      </div>
      <div
        class="bg-white group-hover:opacity-0 opacity-100 transition duration-500 group-hover:pointer-events-none space-y-1 py-2"
      >
        <p>{{ item?.name }}</p>
        <p class="text-gray-500">Women's Shoes</p>
        <p class="text-gray-500">3 Colors</p>
        <p class="py-2">{{ activeOption.price }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  item: Object,
});

let activeOptionIndex = ref(0);
let activeOption = computed(() => props.item.options[activeOptionIndex.value]);
</script>

<style></style>