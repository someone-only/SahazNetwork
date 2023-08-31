<script setup lang="ts">
const linkList = ["Home", "About us", "Product", "Review"];
</script>

<template>
  <header class="bg-white py-4 border">
    <nav class="flex justify-between items-center w-[92%] mx-auto">
      <div>
        <h1 class="text-lg md:text-2xl font-bold uppercase">
          sahaz<span
            class="bg-gradient-to-t text-transparent bg-clip-text from-amber-400 to-amber-600"
            >network</span
          >
        </h1>
      </div>
      <div
        class="md:static absolute bg-white md:min-h-fit min-h-[60vh] left-0 top-[-100%] md:w-auto w-full flex items-center justify-center px-4"
      >
        <ul class="flex md:flex-row flex-col md:items-center gap-6 md:gap-8">
          <li
            class="hover:text-slate-300 hover:underline"
            v-for="list in linkList"
          >
            {{ list }}
          </li>
        </ul>
      </div>
      <div>
        <button
          class="bg-amber-400 px-5 py-2 text-white rounded-full hover:bg-amber-600 transition duration-300 ease-in hidden md:block"
        >
          Log In
        </button>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 md:hidden text-amber-500"
          viewBox="0 0 448 512"
        >
          <path
            d="M0 96C0 78.3 14.3 64 32 64H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 128 0 113.7 0 96zM0 256c0-17.7 14.3-32 32-32H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32c-17.7 0-32-14.3-32-32zM448 416c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32H416c17.7 0 32 14.3 32 32z"
          />
        </svg>
      </div>
    </nav>
  </header>
</template>
