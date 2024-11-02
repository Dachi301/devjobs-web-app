<script setup>
// Filter Components
import FormFilterOption from '@/components/filter-bar/FormFilterOption.vue'
import FullTimeFilterCheckbox from '@/components/filter-bar/FullTimeFilterCheckbox.vue'

// Common Components
import PrimaryButton from '@/components/common/buttons/PrimaryButton.vue'
import TextInput from '@/components/common/inputs/TextInput.vue'

// Icons
import SearchIcon from '@/components/icons/SearchIcon.vue'
import LocationIcon from '@/components/icons/LocationIcon.vue'
</script>

<template>
    <form @submit.prevent class="h-20 rounded-[6px] flex">
        <FormFilterOption class="grow-[3]">
            <TextInput
                class="pl-[72px] rounded-l-[6px]"
                placeholder="Filter by title, companies, expertise…"
            />
            <SearchIcon class-name="absolute top-7 left-8" />
        </FormFilterOption>
        <FormFilterOption class="grow-[1]">
            <TextInput
                class="pl-[56px]"
                placeholder="Filter by title, companies, expertise…"
            />
            <LocationIcon class="absolute top-7 left-[23px]" />
        </FormFilterOption>
        <FormFilterOption class="bg-white rounded-r-[6px]">
            <div class="flex items-center pr-4">
                <FullTimeFilterCheckbox />
                <PrimaryButton type="submit" text-value="Search" />
            </div>
        </FormFilterOption>
    </form>
</template>
