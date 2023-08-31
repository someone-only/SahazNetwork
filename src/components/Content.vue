<template>
  <div data-aos="fade-right">
    <div>
      <slot name="title"></slot>
    </div>
    <div class="mx-6 my-6">
      <p>
        <slot name="paragraf1"></slot>
      </p>
    </div>
    <div class="mx-6 my-6">
      <p>
        <span class="font-bold text-lg">
          <slot name="subTitle"></slot>
        </span>
        <slot name="paragraf2"></slot>
      </p>
    </div>
  </div>
  <div class="flex justify-center mx-auto my-6" data-aos="fade-right">
    <button
      class="py-2 px-6 rounded-full bg-amber-400 text-white hover:bg-white hover:ring-1 hover:ring-slate-900 hover:text-slate-900 hover:underline transition duration-300 ease-in"
    >
      Beli Sekarang
    </button>
  </div>
</template>
