<template>
  <div class="slidev-layout intro p-0 opacity-100" :style="image ? style : ''">
    <div class="absolute h-full w-full bg-black opacity-55"></div>
    <div class="h-full">
      <slot />
    </div>
  </div>
</template>
<script setup lang="ts">
import { computed, defineProps } from "vue";
import { handleBackground } from "../utils";
const props = defineProps({
  image: {
    type: String,
    required: false,
  },
});
const style = computed(() => handleBackground(props.image));
</script>
