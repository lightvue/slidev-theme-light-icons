<template>
  <div class="relative h-full intro grid grid-cols-12">
    <div class="absolute h-full w-full" style="z-index: -10">
      <backgroundBubble />
    </div>
    <div
      v-if="image"
      :class="[equal ? 'col-span-6' : 'col-span-4', 'my-auto h-full']"
    >
      <img :src="image" />
    </div>
    <div
      :class="[
        'slidev-layout my-auto',
        image ? 'col-span-6' : 'col-span-12',
        equal ? 'col-span-6' : 'col-span-8',
      ]"
    >
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts">
// Dependencies
import { defineProps } from "vue";

const props = defineProps({
  image: {
    type: String,
    required: false,
  },
  equal: {
    type: Boolean,
    default: false,
    required: false,
  },
});
</script>
