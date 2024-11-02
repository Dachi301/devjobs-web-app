<script setup>
import DevjobsLogo from '@/assets/images/desktop/logo.svg'
import SunIcon from '@/assets/images/desktop/icon-sun.svg'
import MoonIcon from '@/assets/images/desktop/icon-moon.svg'
</script>

<template>
    <header>
        <div class="flex justify-between items-center pt-16 px-48">
            <img :src="DevjobsLogo" alt="Dev-jobs Logo" />
            <div class="flex items-center gap-5">
                <img :src="SunIcon" alt="Sun Icon" />
                <label class="inline-flex items-center cursor-pointer">
                    <input type="checkbox" value="" class="sr-only peer" />
                    <div
                        class="relative w-12 h-6 bg-white peer-focus:outline-none rounded-full peer peer-checked:after:translate-x-[22px] rtl:peer-checked:after:-translate-x-full after:content-[''] after:absolute after:top-[5px] after:start-[6px] after:bg-[#5964E0] after:hover:bg-[#939BF4] after:rounded-full after:h-[14px] after:w-[14px] after:transition-all dark:border-gray-600"
                    />
                </label>
                <img :src="MoonIcon" alt="Sun Icon" />
            </div>
        </div>
    </header>
</template>

<style scoped></style>
