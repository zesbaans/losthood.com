<script setup lang="ts">
useHead({
  titleTemplate: (title) => (title ? `${title} — Lost Hood` : "Lost Hood"),
  htmlAttrs: { lang: "en" },
})
</script>

<template>
  <NuxtPage />
</template>

<style>
html,
body {
  margin: 0;
  background: #1d1426;
  color: #f5f5f5;
  font-family:
    system-ui,
    -apple-system,
    "Segoe UI",
    Roboto,
    sans-serif;
}
</style>
