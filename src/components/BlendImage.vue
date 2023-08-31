<template>
  <div class="group relative w-full h-full overflow-hidden" style="width: 100%; height: 350px;">
    <div class="w-full h-full">
      <slot name="img"
        ><img
          class="object-cover w-full h-full"
          src="https://source.unsplash.com/400x350?city"
          alt=""
      /></slot>
      <slot
        ><div
          class="absolute inset-0 bg-gradient-to-t from-transparent to-white from-60%"
        ></div>
      </slot>
    </div>
  </div>
</template>
