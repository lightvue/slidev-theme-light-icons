<template>
    <i :class="`light-icon-${icon}`" :style="`font-size: ${size}`"/>
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
        default: '16px'
    }
});
</script>