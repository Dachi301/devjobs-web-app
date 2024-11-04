<script setup>
import { defineProps } from 'vue'

defineProps({
    time: String,
    jobType: String,
    title: String,
    company: String,
    location: String,
})
</script>

<template>
    <div class="relative bg-white pt-12 pb-8 px-8 rounded-[6px]">
        <slot name="icon" />
        <div class="flex flex-col gap-4 pb-11">
            <div class="flex items-baseline gap-3 text-[#6E8098]">
                <h2>{{ time }}</h2>
                <div class="w-1 h-1 bg-[#6E8098] rounded-[50%]" />
                <h2>{{ jobType }}</h2>
            </div>
            <h1 class="text-[#19202D] text-[20px] font-bold">{{ title }}</h1>
            <div class="text-[#6E8098]">{{ company }}</div>
        </div>
        <div class="text-[#5964E0] text-sm font-bold">{{ location }}</div>
    </div>
</template>
