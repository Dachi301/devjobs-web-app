<script setup>
import { defineProps } from 'vue'

defineProps({
    textValue: {
        type: String,
        default: '',
    },
    type: String,
    onClick: Function,
})
</script>

<template>
    <button
        @click="onClick"
        :type="type"
        class="bg-[#5964E0] hover:bg-[#939BF4] transition-all min-w-32 py-4 px-7 rounded-[5px] text-white font-bold"
    >
        {{ textValue }}
    </button>
</template>
