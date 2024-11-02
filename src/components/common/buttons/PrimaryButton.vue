<script setup>
import { defineProps } from 'vue'

defineProps({
    textValue: {
        type: String,
        default: '',
    },
    type: String,
})
</script>

<template>
    <button
        :type="type"
        class="bg-[#5964E0] hover:bg-[#939BF4] transition-all min-w-[123px] py-4 px-7 rounded-[5px] text-white font-bold"
    >
        {{ textValue }}
    </button>
</template>
