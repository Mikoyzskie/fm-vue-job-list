<script setup lang="ts">
defineProps<{
  text: string
  isNew?: boolean
  isFeatured?: boolean
}>()
</script>

<template>
  <span class="badge" :class="{ new: isNew, featured: isFeatured }">{{ text }}</span>
</template>

<style>
.badge {
  font-size: 14px;
  font-weight: 700;
  border-radius: 50px;
  padding: 7px 8px 3px;
  color: var(--white);
  letter-spacing: -0.11px;
}

.new {
  background: var(--primary);
}

.featured {
  background: var(--dark-grayish-cyan);
}
</style>
