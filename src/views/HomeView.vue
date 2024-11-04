<script setup>
import FilterBarRoot from '@/components/filter-bar/FilterBarRoot.vue'
import JobListings from '@/components/job-listings/JobListings.vue'
</script>

<template>
    <main class="px-48 mt-14">
        <FilterBarRoot />
        <JobListings :limit="12" />
    </main>
</template>
