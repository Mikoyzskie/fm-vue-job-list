<script setup lang="ts">
defineProps<{
  text: string
}>()
</script>

<template>
  <button class="filter-button">{{ text }}</button>
</template>

<style>
.filter-button {
  all: unset;
  color: var(--primary);
  font-weight: 700;
  font-size: 16px;
  background-color: var(--filter-table);
  border-radius: 4px;
  padding: 5px 11px 3px;
}
</style>
