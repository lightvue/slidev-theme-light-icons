<template>
  <div
    class="inline-flex justify-center items-center p-3 rounded-full text-white"
    :style="{
      backgroundColor: '#009286',
      boxShadow: '0px 0px 10px rgb(6,228,210,0.5)',
    }"
  >
    <slot />
  </div>
</template>

<script setup lang="ts">
import { defineProps } from "vue";
const props = defineProps({});
</script>