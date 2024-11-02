<script setup>
import { RouterView } from 'vue-router'
import Header from '@/components/header/Header.vue'
</script>

<template>
    <div class="header-bg"></div>
    <Header />
    <RouterView />
</template>

<style>
.header-bg {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 12rem;
    border-radius: 0 0 0 100px;
    background-image: url('@/assets/images/desktop/bg-pattern-header.svg');
    background-size: cover;
    background-repeat: no-repeat;
    z-index: -1;
}
</style>
<!--position: absolute;-->
<!--top: 0;-->
<!--left: 0;-->
<!--width: 100%;-->
<!--height: 16rem;-->
<!--border-radius: 0 0 0 var(&#45;&#45;border-radius-xl);-->
<!--background-image: url(/static/media/bg-pattern-header.f3307602.svg);-->
<!--background-repeat: no-repeat;-->
<!--background-size: cover;-->
<!--}-->
