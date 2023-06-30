<script setup lang="ts">
import { computed } from "vue";

const props = defineProps({
  maxWidth: {
    type: String as () => "full" | "xs" | "sm" | "md" | "lg" | "xl",
    default: "full",
  },
  border: {
    type: Boolean,
    default: true,
  },
  backgroundColor: {
    type: String as () => "base",
    default: "base",
  },
});

const width = computed(() => {
  if (props.maxWidth != "full") {
    return "max-w-" + props.maxWidth;
  } else {
    return "w-full";
  }
});

const border = computed(() => {
  if (props.border) {
    return "border border-neutral-200/60 shadow-sm";
  }
});

const styles = computed(() => {
  return `${width.value} ${border.value}`;
});
</script>

<template>
  <div :class="[styles]" class="overflow-hidden rounded-lg">
    <slot name="image" />

    <div class="p-7">
      <div class="mb-2 text-lg font-bold leading-none tracking-tight">
        <slot name="card-title" />
      </div>

      <div
        v-if="$slots['card-body']"
        class="text-neutral-500"
        :class="{ 'mb-5': $slots['card-actions'] }"
      >
        <slot name="card-body" />
      </div>

      <div v-if="$slots['card-actions']" class="flex gap-2">
        <slot name="card-actions" />
      </div>
    </div>

    <slot />
  </div>
</template>
