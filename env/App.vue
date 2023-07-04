<script setup lang="ts">
import { ref } from "vue";
import PVTabs from "./../src/components/PVTabs.vue";

const tab = ref(0);
</script>

<template>
  <div class="container mx-auto p-2 sm:p-0">
    <h1 class="mb-16 text-center text-4xl font-bold text-red-500">DEV ENV</h1>

    <PVTabs
      v-model="tab"
      :items="[
        { title: 'Test' },
        { title: 'Bruh' },
        { title: 'Das ist der zweite Test' },
      ]"
      max-width="xs"
    />
  </div>
</template>
