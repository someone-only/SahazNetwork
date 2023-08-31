<script setup lang="ts">
const paketan = [
  {
    speed: "100Mbps",
    price: "Rp.399.000",
    benefit: [
      "Diskon Biaya PSB 70%",
      "Kecepatan internet up to 100 Mbps",
      "Disney Plus Hotstar",
    ],
  },
  {
    speed: "200Mbps",
    price: "Rp.699.000",
    benefit: [
      "Diskon Biaya PSB 70%",
      "Kecepatan internet up to 200 Mbps",
      "Disney Plus Hotstar",
    ],
  },
  {
    speed: "250Mbps",
    price: "Rp.999.000",
    benefit: [
      "Diskon Biaya PSB 70%",
      "Kecepatan internet up to 250 Mbps",
      "Disney Plus Hotstar",
    ],
  }, 
];
</script>
<template>
  <div
    class="flex flex-wrap flex-col md:flex-row gap-4 justify-center items-center my-6 mx-6"
  >
    <div
      data-aos="fade-right"
      class="bg-white p-6 rounded-md shadow-lg"
      v-for="{ speed, price, benefit } in paketan"
    >
      <div>
        <p class="text-base text-slate-400">Speed</p>
      </div>
      <div class="my-2">
        <h1 class="text-3xl text-slate-900 font-bold">{{ speed }}</h1>
      </div>
      <div class="my-2">
        <h1 class="text-xl font-bold text-slate-900">
          {{ price }}<span class="text-slate-400">/bulan</span>
        </h1>
      </div>
      <div>
        <p class="text-base font-bold text-slate-400 my-1">Benefit</p>
      </div>

      <div class="mx-4 mb-2">
        <ul>
          <li class="text-slate-900 list-disc" v-for="item in benefit">
            {{ item }}
          </li>
        </ul>
      </div>
      <div class="flex justify-center items-center mx-auto my-2">
        <button
          class="py-2 px-6 rounded-full bg-amber-400 text-white hover:bg-white hover:ring-1 hover:ring-slate-900 hover:text-slate-900 hover:underline transition duration-300 ease-in"
        >
          Beli Sekarang
        </button>
      </div>
    </div>
  </div>
</template>
