<template>
  <div
    class="
      flex
      space-x-3
      py-7
      px-7
      
      justify-around
      items-center
      text-sm
      tracking-wider
    "
  >
    <div class="">
      <svg
        aria-hidden="true"
        class="pre-logo-svg"
        focusable="false"
        viewBox="0 0 24 24"
        role="img"
        width="60px"
        height="60px"
        fill="none"
      >
        <path
          fill="currentColor"
          fill-rule="evenodd"
          d="M21 8.719L7.836 14.303C6.74 14.768 5.818 15 5.075 15c-.836 0-1.445-.295-1.819-.884-.485-.76-.273-1.982.559-3.272.494-.754 1.122-1.446 1.734-2.108-.144.234-1.415 2.349-.025 3.345.275.2.666.298 1.147.298.386 0 .829-.063 1.316-.19L21 8.719z"
          clip-rule="evenodd"
        ></path>
      </svg>
    </div>
    <div class="flex space-x-3 items-center uppercase">
      <p class="font-bold border-b-4 border-black">man</p>
      <p class="font-light text-gray-600">women</p>
    </div>
    <form class="w-1/5">
      <div class="relative mx-auto max-w-lg">
        <input
          type="text"
          placeholder="search ..."
          class="
            cursor-pointer
            focus:cursor-text
            peer
            relative
            z-10
            h-12
            w-12
            rounded-full
            border
            bg-transparent
            pl-12
            outline-none
            duration-300
            delay-150
            ease-out
            focus:w-full focus:border-gray-500 focus:pl-16 focus:transition
          "
        />
         <div class="invisible peer-focus:visible peer-focus:transition duration-300 absolute border rounded shadow-lg border-gray-50  bg-white w-full z-50 py-6">
           <div class="px-6 space-y-4">
             
             <p class="tracking text-gray-400">Popular Search Terms</p>
             <hr>
             <p>Air Force 1</p>
             <p>Jordan</p>
             <p>Air max</p>
             <p>Blazer</p>
             <p>Gifts</p>
            </div>
         </div>
         
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="
            absolute
            inset-y-0
            my-auto
            h-8
            w-12
            border-r border-transparent
            stroke-gray-500
            p-2
            peer-focus:border-gray-500 peer-focus:stroke-gray-900
          "
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
          />
        </svg>
      </div>
    </form>
    <div class="flex space-x-7">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="w-6 h-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"
        />
      </svg>

      <div class="relative">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-6 h-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12z"
          />
        </svg>
        <div class="absolute -top-1 -right-3">
          <p
            class="
              bg-red-500
              h-4
              w-4
              rounded-full
              text-white
              flex
              justify-center
              items-center
              p-2.5
            "
          >
            7
          </p>
        </div>
      </div>

      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="w-6 h-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z"
        />
      </svg>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>