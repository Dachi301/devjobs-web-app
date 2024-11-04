<script setup>
import ScootLogoIcon from '@/assets/images/logos/scoot.svg'

import { defineProps } from 'vue'

defineProps({
    className: String,
})
</script>

<template>
    <img alt="Scoot Logo" :class="className" :src="ScootLogoIcon" />
</template>
