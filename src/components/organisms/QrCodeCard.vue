<template>
  <div class="qr-code__card">
    <div class="qr-code__image-wrapper">
      <img class="qr-code__image" src="@/assets/images/image-qr-code.png" alt="QR Code" />
    </div>
    <div class="qr-code__text">
      <h1 class="qr-code__title">
        <slot name="title"></slot>
      </h1>
      <p class="qr-code__description">
        <slot name="description"></slot>
      </p>
    </div>
  </div>
</template>

<style scoped>
.qr-code__card {
  background-color: var(--color-white);
  border-radius: 20px;
  padding: 16px;
  text-align: center;
  max-width: 320px;
}

.qr-code__image-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}

.qr-code__image {
  width: 100%;
  border-radius: 10px;
  display: block;
}

.qr-code__text {
  margin-top: 24px;
  display: flex;
  flex-direction: column;
  padding: 0 16px;
  gap: 16px;
}

.qr-code__title {
  color: var(--color-dark-blue);
  font: var(--text-preset-1);
}

.qr-code__description {
  color: var(--color-slate-500);
  font: var(--text-preset-2);
}
</style>