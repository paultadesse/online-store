<template>
  <div class="justify-center py-12 flex flex-wrap gap-2">
    <a
      href="#"
      class="group"
      v-for="(item, itemIndex) in items"
      :key="itemIndex"
    >
      <ItemInfo :item="item" />
    </a>
  </div>
</template>

<script setup>
const props = defineProps({
  items: Array,
});
// const props = computed(() => items)
let activeItemIndex = ref(0);

function updateItems(item, option) {
  console.log(item.includes(option));
}
</script>

<style>
</style>