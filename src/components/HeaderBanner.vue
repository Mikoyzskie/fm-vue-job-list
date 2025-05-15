<template>
  <header>
    <img src="@/assets/bg-header-mobile.svg" height="156" alt="" class="header-img mobile" />
    <img src="@/assets/bg-header-desktop.svg" height="156" alt="" class="header-img desktop" />
  </header>
</template>

<style scoped>
header {
  height: 156px;
  width: 100%;
  background-color: var(--primary);
}

.header-img {
  width: 100%;
  object-fit: cover;
}

.mobile {
  display: block;
}

.desktop {
  display: none;
}

@media only screen and (min-width: 375px) {
  .mobile {
    display: none;
  }
  .desktop {
    display: block;
  }
}
</style>
