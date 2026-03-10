# Frontend Mentor - QR code component solution

This is my solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). I originally built this challenge earlier as a simple HTML & CSS exercise.
For this iteration, I rebuilt it using Vue to practice component structure and slots, while keeping the design faithful to the original challenge.

The goal of this version was not only to recreate the layout, but also to explore how small UI components can be structured in a component-based architecture.

## Table of contents

- [Frontend Mentor - QR code component solution](#frontend-mentor---qr-code-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)

## Overview

### Screenshot

![Screenshot](./src/assets/images/screenshot.png)

### Links

- Solution URL: [Frontend Mentor solution](https://github.com/arne-witteler/qr-code-component-vue)
- Live Site URL: [Live demo](https://qr-code-component-vue-beryl.vercel.app)

## My process

### Built with

- Vue 3
- Vite
- Semantic HTML 5
- CSS custom properties
- Flexbox
- Mobile-first workflow
- component-based architecture
- Vue slots for flexible content composition

### What I learned

Since I had already completed this challenge once using plain HTML and CSS, this version focused on exploring a Vue-based implementation.

Key things I practiced in this iteration:
- Structuring UI using Vue components
- Using slots to pass flexible content into reusable components
- Separating layout components from content
- Organizing files using a small atomic-style structure (molecules / organisms)

For example, the QrCodeCard component exposes slots for the title and description so the layout stays reusable while the text content can change.

```
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
```

This approach helps keep layout, styling, and content responsibilities clearly separated.