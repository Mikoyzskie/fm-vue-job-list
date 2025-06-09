<script setup lang="ts">
import HeaderBanner from './components/HeaderBanner.vue'
import JobCard from './components/JobCard.vue'
</script>

<template>
  <HeaderBanner />
  <div class="container">
    <JobCard />
    <JobCard />
    <JobCard />
    <JobCard />
    <JobCard />
  </div>
</template>

<style scoped>
.container {
  width: 100%;
  max-width: 1158px;
  padding: 56px 24px 34px 24px;
  display: flex;
  flex-direction: column;
  gap: 40px;
}
</style>
