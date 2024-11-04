<script setup>
import { RouterView } from 'vue-router'

import Header from '@/components/header/Header.vue'
import BackgroundHeaderImage from '@/components/header/BackgroundHeaderImage.vue'
</script>

<template>
    <BackgroundHeaderImage />
    <Header />
    <RouterView />
</template>
