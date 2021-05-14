<template>
  <div class="layout-name absolute text-xs">
    <span v-if="layoutName">
      Layout
      <span class="text-primary dark:text-primary-lighter"> {{layoutName}}</span>
      <span> &nbsp;<light-icon icon="bulb" size="20px"/> </span>
    </span>
    <slot v-else></slot>
  </div>
</template>
<script setup lang="ts">
import { defineProps } from "vue";
const props = defineProps({
    layoutName: {
        type: String,
    },
});
</script>
<style>
.layout-name {
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
  padding: 8px 12px;
  cursor: pointer;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
  border-radius: 4px;
  background-color: #e5f2f2;
  /* box-shadow: 0px 0px 30px rgba(107, 106, 106, 0.2), 0px 0px 10px rgba(107, 106, 106, 0.1); */
  /* color: #ffffff; */
}
.layout-name:hover {
  opacity: 1;
}
.dark .layout-name {
  background-color: rgba(15, 41, 39, 0.9);
  /* box-shadow: 0px 0px 30px rgba(199, 199, 199, 0.042), 0px 0px 10px rgba(107, 106, 106, 0.08); */
}
</style>
