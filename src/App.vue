<script setup lang="ts">
import HeaderBanner from './components/HeaderBanner.vue'
import JobCard from './components/JobCard.vue'
</script>

<template>
  <HeaderBanner />
  <div class="container">
    <JobCard />
  </div>
</template>

<style scoped>
.container {
  width: 100%;
  max-width: 1158px;
  padding: 32px 24px 34px 24px;
}
</style>
