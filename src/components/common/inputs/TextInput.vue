<script setup>
import { defineProps } from 'vue'

defineProps({
    placeholder: String,
    className: String,
})
</script>

<template>
    <input
        type="text"
        :placeholder="placeholder"
        :class="`w-full flex items-center gap-4 py-7 border-r outline-0 ${className}`"
    />
</template>
