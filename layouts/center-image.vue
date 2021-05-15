<template>
  <div class="relative h-full w-full intro grid grid-cols-12">
    <div class="absolute h-full w-full" style="z-index: -10">
      <BubbleFrame v-if="!hideFrame"/>
    </div>
    <div class="col-span-12 m-auto">
      <div class="text-center">
        <slot />
      </div>
      <div v-if="image" class="m-auto w-8/12 rounded-lg manual-shadow">
        <img :src="image" class="rounded-lg" />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import { defineProps } from "vue";
const props = defineProps({
  image: {
    type: String,
    required: false,
  },
  hideFrame: {
    type: Boolean,
    default: false,
  }
});
</script>