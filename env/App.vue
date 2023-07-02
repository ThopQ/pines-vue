<script setup lang="ts">
import PVCard from "./../src/components/PVCard.vue";
import PVButton from "./../src/components/PVButton.vue";
</script>

<template>
  <div class="container mx-auto p-2 sm:p-0">
    <h1 class="mb-16 text-center text-4xl font-bold text-red-500">DEV ENV</h1>

    <div class="mb-4 grid grid-cols-1 gap-4 md:grid-cols-2">
      <PVCard>
        <template #media>
          <img
            src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2370&q=80"
            class="object-cover sm:rounded-lg"
          />
        </template>

        <template #title>
          <h3>This is a working card</h3>
        </template>

        <template #body>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
            ue enim ab vel, magni omnis quasi dignissimos vitae dicta voluptate
            necessitatibus adipisci sequi. Lorem, ipsum dolor sit amet Lorem
            ipsum dolor sit amet consectetur adipisicing elit. Blanditiis ue
            enim ab vel, magni omnis quasi dignissimos vitae dicta voluptate
            necessitatibus adipisci sequi. Lorem, ipsum dolor sit amet Lorem
            ipsum dolor sit amet consectetur adipisicing elit. Blanditiis ue
            enim ab vel, magni omnis quasi dignissimos vitae dicta voluptate
            necessitatibus adipisci sequi. Lorem, ipsum dolor sit amet
          </p>
        </template>

        <template #actions>
          <PVButton block>Test</PVButton>
        </template>
      </PVCard>

      <div class="flex h-full flex-col gap-4">
        <PVCard>
          <template #title>
            <h3>This is a working card</h3>
          </template>

          <template #body>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Blanditiis ue enim ab vel, magni omnis quasi dignissimos vitae
              dicta voluptate necessitatibus adipisci sequi. Lorem, ipsum dolor
              sit amet Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Blanditiis ue enim ab vel, magni omnis quasi dignissimos vitae
              dicta voluptate necessitatibus
            </p>
          </template>

          <template #actions>
            <PVButton>Test</PVButton>
            <PVButton color="error" secondary>Test</PVButton>
          </template>
        </PVCard>

        <PVCard>
          <template #media>
            <img
              src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2370&q=80"
              class="object-cover"
            />
          </template>
        </PVCard>
      </div>
    </div>

    <PVCard horizontal>
      <template #media>
        <img
          src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2370&q=80"
          class="object-cover sm:rounded-lg md:max-w-xs"
        />
      </template>

      <template #title>
        <h3>This is a working card</h3>
      </template>

      <template #body>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis ue
          enim ab vel, magni omnis quasi dignissimos vitae dicta voluptate
          necessitatibus adipisci sequi. Lorem, ipsum dolor sit amet Lorem ipsum
          dolor sit amet consectetur adipisicing elit. Blanditiis ue enim ab
          vel, magni omnis quasi dignissimos vitae dicta voluptate
          necessitatibus adipisci sequi. Lorem, ipsum dolor sit amet Lorem ipsum
          dolor sit amet consectetur adipisicing elit. Blanditiis ue enim ab
          vel, magni omnis quasi dignissimos vitae dicta voluptate
          necessitatibus adipisci sequi. Lorem, ipsum dolor sit amet
        </p>
      </template>

      <template #actions>
        <PVButton>Test</PVButton>
        <PVButton color="error" secondary>Test</PVButton>
      </template>
    </PVCard>
  </div>
</template>
