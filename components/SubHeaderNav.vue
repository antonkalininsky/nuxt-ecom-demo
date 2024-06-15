<script setup lang="ts">
const props = defineProps({
  hasNav: {
    type: Boolean,
    default: false,
  },
  title: {
    type: String,
    default: "Заголовок",
  },
  subtitle: {
    type: String,
    default: "",
  },
});
</script>

<template>
  <div class="flex justify-between items-center py-2">
    <div class="flex items-start gap-x-1">
      <div class="font-bold">{{ props.title }}</div>
      <div v-if="$props.subtitle" class="text-xs text-gray-500">
        {{ $props.subtitle }}
      </div>
    </div>
    <div class="flex gap-x-2" v-if="props.hasNav">
      <Button
        class="border-2 rounded-full p-1 w-8 h-8 flex justify-center items-center"
      >
        <Icon class="text-gray-400" name="mingcute:left-fill" />
      </Button>
      <Button
        class="border-2 rounded-full p-1 w-8 h-8 flex justify-center items-center"
      >
        <Icon class="text-gray-400" name="mingcute:right-fill" />
      </Button>
    </div>
  </div>
</template>
