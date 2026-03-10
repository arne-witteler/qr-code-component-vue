<template>
  <div class="attribution">
    <p class="attribution__text">
      <slot name="credit"></slot>
    </p>
  </div>
</template>

<style scoped>
.attribution__text {
  margin-top: 12px;
  font: var(--text-preset-3);
}
</style>