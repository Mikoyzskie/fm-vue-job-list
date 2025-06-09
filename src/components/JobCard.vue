<script setup lang="ts">
import BadgeIcon from './BadgeIcon.vue'
import FilterButton from './FilterButton.vue'
</script>

<template>
  <div class="item-container">
    <img src="../assets/insure.svg" class="company-logo" />
    <div class="wrapper">
      <div class="details">
        <div class="details-header">
          <span class="company">Company</span>
          <div class="badge-group">
            <BadgeIcon text="NEW!" :is-new="true" />
            <BadgeIcon text="FEATURED" :is-featured="true" />
          </div>
        </div>
        <span class="title">Senior Frontend Developer</span>
        <div class="details-footer">
          <span class="gray-text">1d ago</span>
          <div class="circle-spacer"></div>
          <span class="gray-text">Full Time</span>
          <div class="circle-spacer"></div>
          <span class="gray-text">USA only</span>
        </div>
      </div>
      <div class="separator"></div>
      <div class="filter-container">
        <FilterButton text="Frontend" />
        <FilterButton text="Senior" />
        <FilterButton text="HTML" />
        <FilterButton text="CSS" />
        <FilterButton text="Javascript" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.item-container {
  background: var(--white);
  border-radius: 5px;
  filter: drop-shadow(0 10px 10px rgba(91, 164, 164, 0.25));
  position: relative;
}

.company-logo {
  position: absolute;
  height: 48px;
  width: 48px;
  left: 24px;
  top: -24px;
}

.details-header {
  display: flex;
  align-items: center;
  gap: 33px;
}

.badge-group {
  display: flex;
  gap: 8px;
}

.details {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.wrapper {
  border-left: 5px solid var(--primary);
  width: 100%;
  border-radius: 5px;
  padding: 32px 24px 24px 19px;
}

.company {
  color: var(--primary);
  font-size: 13px;
  font-weight: 700;
}

.title {
  color: var(--dark-grayish-cyan);
  font-weight: 700;
  line-height: 24px;
}

.circle-spacer {
  background-color: var(--grayish-cyan);
  height: 4px;
  width: 4px;
  border-radius: 100%;
}

.gray-text {
  color: var(--grayish-cyan);
  font-size: 16px;
  letter-spacing: -0.12px;
  line-height: 24px;
}

.details-footer {
  display: flex;
  align-items: center;
  gap: 10px;
}

.separator {
  height: 1px;
  background-color: hsl(180, 10%, 74%);
  width: 100%;
  margin-top: 16px;
}

.filter-container {
  display: flex;
  align-items: center;
  gap: 16px;
  flex-wrap: wrap;
  margin-top: 16px;
}
</style>
