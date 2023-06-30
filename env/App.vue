<script setup lang="ts">
import PVCard from "./../src/components/PVCard.vue";
import PVButton from "./../src/components/PVButton.vue";
</script>

<template>
  <div>
    <h1 class="mb-16 text-center text-4xl font-bold text-red-500">DEV ENV</h1>

    <PVCard max-width="sm">
      <template #card-title>
        <h3>Test</h3>
      </template>

      <template #card-body>
        <p>Das ist ein Test</p>
      </template>

      <template #card-actions>
        <PVButton>Card Button</PVButton>
      </template>
    </PVCard>
  </div>
</template>
