<script setup lang="ts">
import { RouterLink } from "vue-router";
</script>

<template>
  <section class="bg-white dark:bg-gray-900">
    <div class="py-8 px-4 mx-auto max-w-screen-xl text-center lg:py-16">
      <h1
        class="mb-4 text-3xl font-extrabold tracking-tight leading-none text-primary-100 md:text-5xl lg:text-6xl dark:text-white"
      >
        #InternetSuperCepat
      </h1>
      <p
        class="mb-8 text-lg font-normal text-gray-500 lg:text-xl sm:px-16 lg:px-48 dark:text-gray-400"
      >
        Terhubung dengan kecepatan tanpa batas. Jelajahi dunia digital dengan
        layanan internet terbaik untuk pengalaman online yang luar biasa bersama
        <span class="font-bold">SahazNetwork!</span>
      </p>
      <div
        class="flex flex-col space-y-4 sm:flex-row sm:justify-center sm:space-y-0"
      >
        <RouterLink
          to="/SahazNetwork/price"
          class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-white rounded-lg bg-primary-100 hover:bg-primary-200 focus:ring-4 focus:ring-primry-200 dark:focus:ring-blue-900"
        >
          Beli Sekarang
          <svg
            class="w-3.5 h-3.5 ms-2 rtl:rotate-180"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 14 10"
          >
            <path
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M1 5h12m0 0L9 1m4 4L9 9"
            />
          </svg>
        </RouterLink>
        <RouterLink
          to="SahazNetwork/about"
          class="inline-flex justify-center items-center py-3 px-5 sm:ms-4 text-base font-medium text-center text-gray-900 rounded-lg border border-gray-300 hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800"
        >
          Pelajari Lebih Lanjut
        </RouterLink>
      </div>
    </div>
  </section>
</template>
