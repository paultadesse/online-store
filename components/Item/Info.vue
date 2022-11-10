<template>
  <div>
    <img :src="activeItemImage" alt="" />
    <div class="py-2 gap-2 hidden group-hover:block">
      <div class="gap-2 flex">
        <div v-for="(option, index) in item[0].options" :key="option.id">
          <img
            class="h-12 w-12"
            :src="option.imgPath"
            alt=""
            @mouseenter="
              (activeItemImage = option.imgPath), 
              (activeItemIndex = index)
            "
          />
        </div>
      </div>
      <div class="space-y-1 py-2">
        <p class="">
          {{ item[0]?.options[activeItemIndex].price }}
          <span class="text-gray-500 line-through px-1">$100</span>
        </p>
        <p class="py-2 text-green-600">14 % off</p>
      </div>
    </div>
    <div class="bg-white group-hover:hidden space-y-1 py-2">
      <p>{{ item[0]?.name }}</p>
      <p class="text-gray-500">Women's Shoes</p>
      <p class="text-gray-500">3 Colors</p>
      <p class="py-2">{{ item[0]?.options[activeItemIndex].price }}</p>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  item: Array,
});

let activeItemImage = ref(props.item[0]?.options[0]?.imgPath);
let activeItemIndex = ref(0);
</script>

<style>
</style>