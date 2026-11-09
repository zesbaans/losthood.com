<script setup lang="ts">
useHead({
  titleTemplate: (title) => (title ? `${title} — Lost Hood` : "Lost Hood"),
  htmlAttrs: { lang: "en" },
  link: [
    { rel: "icon", href: "/favicon.ico?v=2", sizes: "48x48" },
    {
      rel: "icon",
      type: "image/png",
      href: "/favicon-32x32.png?v=2",
      sizes: "32x32",
    },
    { rel: "apple-touch-icon", href: "/apple-touch-icon.png?v=2" },
  ],
})
</script>

<template>
  <NuxtPage />
</template>

<style>
html,
body {
  margin: 0;
  background: #15191b;
  color: #f5f5f5;
  font-family:
    system-ui,
    -apple-system,
    "Segoe UI",
    Roboto,
    sans-serif;
}
</style>
