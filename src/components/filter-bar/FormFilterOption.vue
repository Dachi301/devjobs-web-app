<script setup>
import { defineProps } from 'vue'

defineProps({
    className: {
        type: String,
        default: '',
    },
})
</script>

<template>
    <div :class="`relative ${className}`">
        <slot />
    </div>
</template>
