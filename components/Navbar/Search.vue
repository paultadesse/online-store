<template>
    <form>
      <transition
        enter-from-class="  opacity-0"
        enter-to-class=" opacity-100"
        enter-active-class="transition duration-100"
        leave-from-class=" opacity-100"
        leave-to-class="  opacity-0"
        leave-active-class="transition duration-100"
        @after-enter="showSearch = true"
      >
        <div
          v-if="open"
          class="fixed inset-0 bg-white/50 backdrop-blur-lg z-50 px-16 pt-12"
          @click="showSearch = false"
        >
          <transition
            enter-from-class="transform scale-x-0 opacity-0"
            enter-to-class="transform scale-x-100 opacity-100"
            enter-active-class="transition duration-250"
            leave-from-class="transform scale-x-100 opacity-100"
            leave-to-class="transform scale-x-0 opacity-0"
            leave-active-class="transition duration-250"
            @after-leave="open = false"
          >
            <div @click.stop v-if="showSearch">
              <input
                type="text"
                ref="searchInput"
                placeholder="search ..."
                class="relative rounded-full border border-gray-600 px-6 py-4 w-full"
                :class="open ? 'z-50' : ''"
              />
              <div
                class="mt-3 border rounded shadow-lg border-gray-50 bg-white w-full z-50 py-6"
              >
                <div class="px-6 space-y-4">
                  <p class="tracking text-gray-400">Popular Search Terms</p>
                  <hr />
                  <p>Air Force 1</p>
                  <p>Jordan</p>
                  <p>Air max</p>
                  <p>Blazer</p>
                  <p>Gifts</p>
                </div>
              </div>
            </div>
          </transition>
        </div>
      </transition>
      <div class="relative" :class="open ? '' : 'max-w-lg'">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-8 w-8 stroke-gray-500 p-2"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
          @click="open = true"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
          />
        </svg>
      </div>
    </form>
  </template>
  
  <script setup>
  const open = ref(false);
  const showSearch = ref(false);
  const searchInput = ref();
  
  watch(showSearch, (val) => {
    if (val) {
      nextTick(() => searchInput.value?.focus());
    }
  });
  </script>