<script setup lang="ts">
useHead({
  title: "Lost Hood",
  htmlAttrs: { lang: "en" },
  meta: [
    {
      name: "description",
      content: "Lost Hood — available on the App Store and Google Play.",
    },
  ],
})

interface StoreBadge {
  url?: string
  image: string
  alt: string
}

const badges: StoreBadge[] = [
  {
    url: undefined,
    image: "/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg",
    alt: "Download on the App Store",
  },
  {
    url: "https://play.google.com/store/apps/details?id=nl.zesbaans.losthood",
    image: "/GetItOnGooglePlay_Badge_Web_color_English.svg",
    alt: "Get it on Google Play",
  },
]
</script>

<template>
  <main class="landing">
    <h1 class="title">
      <img
        class="app-icon"
        src="/LostHood-1024.webp"
        alt="Lost Hood"
        width="320"
        height="320"
      />
    </h1>
    <div class="badges">
      <template v-for="badge in badges" :key="badge.image">
        <a
          v-if="badge.url"
          class="badge"
          :href="badge.url"
          target="_blank"
          rel="noopener"
        >
          <img :src="badge.image" :alt="badge.alt" height="56" />
        </a>
        <span
          v-else
          class="badge badge--disabled"
          aria-disabled="true"
          title="Coming soon"
        >
          <img :src="badge.image" :alt="`${badge.alt} (coming soon)`" height="56" />
        </span>
      </template>
    </div>
  </main>
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

.landing {
  min-height: 100vh;
  min-height: 100dvh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2.5rem;
  padding: 1.5rem;
  box-sizing: border-box;
  text-align: center;
}

.title {
  margin: 0;
  line-height: 0;
}

.app-icon {
  width: clamp(160px, 60vw, 320px);
  height: auto;
  border-radius: 22.37%;
  box-shadow: 0 12px 40px rgb(0 0 0 / 0.35);
}

.badges {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1rem;
}

.badges img {
  display: block;
  height: 56px;
  width: auto;
  pointer-events: none;
  user-select: none;
  transition: transform 0.15s ease;
}

.badge {
  display: block;
  cursor: pointer;
  border-radius: 10px;
}

a.badge:hover img,
a.badge:focus-visible img {
  transform: translateY(-2px);
}

.badge--disabled {
  cursor: not-allowed;
  opacity: 0.4;
  filter: grayscale(1);
}
</style>
