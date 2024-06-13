<script setup lang="ts">
const props = defineProps({
  isMain: {
    type: Boolean,
    default: false,
  },
});
</script>
<template>
  <div
    class="relative overflow-hidden flex justify-center items-center group cursor-pointer"
  >
    <img
      class="object-cover size-full transition group-hover:scale-110 duration-700 scale-105"
      src="/images/test.jpg"
      alt=""
      srcset=""
    />
    <div class="absolute bottom-5 left-5 right-5 grid grid-cols-2 items-center">
      <div
        class="text-white font-bold"
        :class="{
          'line-clamp-1 text-lg': $props.isMain,
          'line-clamp-2 opacity-0 group-hover:opacity-100 group-hover:translate-y-0 translate-y-4 transition duration-700':
            !$props.isMain,
        }"
      >
        Lorem ipsum dolor sit
      </div>
      <div v-if="!$props.isMain" class="flex justify-end items-center gap-x-1">
        <div class="py-1 px-2 text-white font-semibold border-2 box-border">
          50%
        </div>
        <div class="py-1.5 px-2 bg-blue-600 text-white font-bold">
          <span class="text-black font-normal line-through mr-1">200 P</span>
          <span>100 P</span>
        </div>
      </div>
    </div>
  </div>
</template>
