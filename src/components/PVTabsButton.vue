<script setup lang="ts">
const props = defineProps({
  active: {
    type: Boolean,
    default: false,
  },
});
</script>

<template>
  <button
    type="button"
    class="h-8 w-full cursor-pointer justify-center whitespace-nowrap rounded-md px-3 text-sm font-medium transition-all focus:bg-white focus:shadow focus:outline-black"
    :class="{ 'bg-white shadow': props.active }"
  >
    <slot />
  </button>
</template>
