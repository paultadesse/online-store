<template>
  <div class="space-x-3">
    <div class="flex bg-gray-50 py-4 space-x-3 px-7 uppercase text-sm tracking-wider">
      <NuxtLink to="/">Home</NuxtLink>
      <NuxtLink to="/about">About</NuxtLink>
      <NuxtLink to="/profile">Profile</NuxtLink>
    </div>
    <div class="w-full pt-7">
      <slot />
    </div>
  </div>
</template>

<script>
</script>

