<script setup lang="ts">
import PVCard from "./../src/components/PVCard.vue";
import PVButton from "./../src/components/PVButton.vue";
</script>

<template>
  <div class="container mx-auto">
    <h1 class="mb-16 text-center text-4xl font-bold text-red-500">DEV ENV</h1>

    <div class="grid grid-cols-2 gap-4">
      <PVCard>
        <template #card-title>
          <h3>Test</h3>
        </template>

        <template #card-body>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
            a saepe nostrum quo exercitationem! Harum ea placeat, nulla ipsa
            aspernatur minus, sunt sed odit libero quo quos hic iusto rem.
          </p>
        </template>

        <template #card-actions>
          <PVButton block>Test</PVButton>
        </template>
      </PVCard>
    </div>
  </div>
</template>
