<script setup>
import SearchIcon from '@/assets/images/desktop/icon-search.svg'

import { defineProps } from 'vue'

defineProps({
    className: String,
})
</script>

<template>
    <img alt="Search Icon" :class="className" :src="SearchIcon" />
</template>
