<script setup>
import JobCard from '@/components/job-listings/JobCard.vue'
import PrimaryButton from '@/components/common/buttons/PrimaryButton.vue'

import { computed, ref } from 'vue'
import jobsData from '@/data.json'

const props = defineProps({
    limit: Number,
    showButton: {
        type: Boolean,
        default: true,
    },
})

const jobs = ref(jobsData)
const currentLimit = ref(props.limit)
const showLoadMoreButton = ref(props.showButton)

const displayedJobs = computed(() => {
    return jobs.value.slice(0, currentLimit.value)
})

const loadMoreButtonIsVisible = computed(() => {
    return showLoadMoreButton.value
})

const showAllJobs = () => {
    currentLimit.value = jobs.value.length
    showLoadMoreButton.value = !showLoadMoreButton.value
}
</script>

<template>
    <div class="grid grid-cols-3 gap-x-7 gap-y-16 mt-24 mb-14">
        <JobCard
            v-for="job in displayedJobs"
            :key="job.id"
            :time="job.postedAt"
            :jobType="job.contract"
            :title="job.position"
            :company="job.company"
            :location="job.location"
        >
            <template v-slot:icon>
                <img
                    alt="Company Logo"
                    :src="job.logo"
                    class="absolute -top-6 left-8"
                />
            </template>
        </JobCard>
    </div>
    <div v-if="loadMoreButtonIsVisible" class="flex justify-center pb-5">
        <PrimaryButton :on-click="showAllJobs" text-value="Load More" />
    </div>
</template>
