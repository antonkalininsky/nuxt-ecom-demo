<script setup lang="ts">
const props = defineProps({
  isActive: {
    type: Boolean,
    default: false,
  },
});
</script>
<template>
  <Button
    class="text-lg py-2 px-5"
    :class="{
      'border-b-2 border-red-500 text-black': props.isActive,
      'text-gray-500 hover:text-red-500 transition': !props.isActive,
    }"
  >
    <slot />
  </Button>
</template>
