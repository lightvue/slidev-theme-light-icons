<template>
  <div class="slidev-layout intro relative grid grid-cols-12">
    <div class="absolute h-full w-full" style="z-index: -10">
      <BubbleFrame v-if="!hideFrame"/>
    </div>
    <div class="my-auto col-span-6 grid grid-cols-12">
      <div class="image col-span-8">
        <img :src="imageHeader" alt="" />
      </div>
      <div class="col-span-12">
        <slot />
      </div>
    </div>
    <div v-if="imageRight" class="my-auto col-span-6 h-full">
      <div class="image">
        <img :src="imageRight" alt="" />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import { defineProps } from "vue";
const props = defineProps({
  imageHeader: {
    type: String,
    required: true,
  },

  imageRight: {
    type: String,
    required: false,
  },
  hideFrame: {
    type: Boolean,
    default: false,
  }
});
</script>

