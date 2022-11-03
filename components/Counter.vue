<template>
  <div>
    <p>{{ count }}</p>
    <button @click="increment">increment</button>
  </div>
</template>

<script setup lang="ts">
let count = ref<number>(20);

function increment(): number {
  // return count.value++
  return count.value++;
}
</script>
