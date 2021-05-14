<template>
    <i :class="`light-icon-${icon}`" :style="`font-size: ${size}; color: ${color}; vertical-align: middle;`"/>
</template>

<script setup lang="ts">
import { defineProps } from "vue";
const props = defineProps({
    icon: {
        type: String,
        default: 'camera'
    },
    size: {
        type: String,
        default: 'inherit'
    },
    color: {
        type: String,
        default: 'inherit'
    },
});
</script>