<script setup>
import CheckIcon from '@/assets/images/desktop/icon-check.svg'
</script>

<template>
    <div class="flex items-center gap-4 py-7 px-8">
        <div class="inline-flex items-center">
            <label class="flex items-center cursor-pointer relative">
                <input
                    type="checkbox"
                    class="peer h-6 w-6 cursor-pointer transition-all bg-[#E7E8E9] appearance-none rounded checked:bg-[#5964E0]"
                    id="check"
                />
                <span
                    class="absolute text-white opacity-0 peer-checked:opacity-100 top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 pointer-events-none"
                >
                    <img alt="Check Icon" :src="CheckIcon" />
                </span>
            </label>
        </div>
        <h1 class="text-[#19202D] font-bold">Full Time Only</h1>
    </div>
</template>
