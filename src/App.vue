<script setup>
import Attribution from './components/molecules/Attribution.vue';
import QrCodeCard from './components/organisms/QrCodeCard.vue';

</script>

<template>
  <div id="app">
    <QrCodeCard>
      <template #image>
        <img src="@/assets/images/image-qr-code.png" alt="QR Code" />
      </template>
      <template #title>
        Improve your front-end skills by building projects
      </template>
      <template #description>
        Scan the QR code to visit Frontend Mentor and take your coding skills to the next level
      </template>
    </QrCodeCard>
    <Attribution>
      <template #credit>
        Challenge by
        <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. Coded by
        <a href="https://github.com/arne-witteler">Arne Witteler</a>.
      </template>
    </Attribution>
  </div>
</template>

<style scoped>
@import '@/assets/styles/main.css';
</style>
