<script setup lang="ts">
import { ref } from "vue";

const links = [
  { name: "Home", url: "/SahazNetwork" },
  { name: "Tentang Kami", url: "/SahazNetwork/about" },
  { name: "Harga", url: "/SahazNetwork/price" },
  { name: "Hubungi Kami", url: "/SahazNetwork/contact" },
];
const isOpen = ref(false);
</script>

<template>
  <nav class="bg-white border-gray-200 dark:bg-gray-900">
    <div
      class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
    >
      <RouterLink
        to="/"
        class="flex items-center space-x-3 rtl:space-x-reverse"
      >
        <span
          class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
          >Sahaz<span
            class="bg-clip-text text-transparent bg-gradient-to-r from-primary-100 to-primary-200"
            >Network</span
          >
        </span>
      </RouterLink>
      <button
        @click="isOpen = !isOpen"
        data-collapse-toggle="navbar-default"
        type="button"
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
        aria-controls="navbar-default"
        aria-expanded="false"
      >
        <span class="sr-only">Open main menu</span>
        <svg
          class="w-5 h-5"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 17 14"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M1 1h15M1 7h15M1 13h15"
          />
        </svg>
      </button>
      <div
        class="w-full md:block md:w-auto"
        :class="{ hidden: !isOpen }"
        id="navbar-default"
      >
        <div
          class="font-medium flex flex-col items-center p-4 md:p-0 mt-4 border border-gray-100 rounded-lg bg-gray-50 md:flex-row md:space-x-8 rtl:space-x-reverse md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700"
        >
          <RouterLink
            :to="url"
            class="px-4 py-2 hover:underline hover:bg-primary-100 hover:text-white hover:rounded-lg"
            v-for="{ name, url } in links"
          >
            {{ name }}
          </RouterLink>
        </div>
      </div>
    </div>
  </nav>
</template>
