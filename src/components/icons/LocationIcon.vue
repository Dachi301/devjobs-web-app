<script setup>
import LocationIcon from '@/assets/images/desktop/icon-location.svg'

import { defineProps } from 'vue'

defineProps({
    className: String,
})
</script>

<template>
    <img alt="Location Icon" :class="className" :src="LocationIcon" />
</template>
