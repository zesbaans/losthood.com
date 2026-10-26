<script setup lang="ts">
useHead({
  title: "Privacy Policy",
  meta: [
    {
      name: "description",
      content: "What data the Lost Hood app collects, how it is used, and what your rights are.",
    },
  ],
})
</script>

<template>
  <main class="privacy">
    <NuxtLink class="back" to="/">← Lost Hood</NuxtLink>

    <h1>Privacy Policy Lost Hood</h1>
    <p class="updated">Last updated: October 2026</p>

    <p>
      Lost Hood is an augmented reality walking experience created by Abner Preis and produced by
      K.O. Productions. This page explains what data the app collects, how it is used, and what
      your rights are as a user.
    </p>
    <p>
      We take privacy seriously. Lost Hood is an art project, not a data business, and we collect
      only what is strictly necessary to make the experience work.
    </p>

    <h2>Who is responsible for your data</h2>
    <p>
      The data controller for Lost Hood is K.O. Productions, Boylestraat 65, 2563 EJ Den Haag,
      The Netherlands (KvK: 85378445). You can reach us at
      <a href="mailto:info@koproductions.nl">info@koproductions.nl</a>.
    </p>

    <h2>What we collect</h2>
    <p>
      Lost Hood uses your device's GPS to determine your position on the Spuistraat. This is how
      the app knows which content to show you at which moment. Location data is processed locally
      on your device and is never stored on our servers or shared with anyone.
    </p>
    <p>
      The app also requires camera access to display augmented reality content. Camera images are
      processed in real time on your device and are never recorded, stored, or transmitted
      anywhere.
    </p>
    <p>
      We do not collect your name, email address, or any other personal information unless you
      contact us directly.
    </p>

    <h2>What we do not collect</h2>
    <p>
      We do not collect or store your location history, images or video from your camera, audio
      recordings, or any identifiable personal data. The app is free, so there is no payment
      information either. We do not access your contacts, photos, or any other apps on your
      device.
    </p>

    <h2>Why we process this data</h2>
    <p>
      Where we process personal data, we do so on the following legal bases under the GDPR:
      legitimate interest (anonymised usage data to improve the app) and consent (location and
      camera access, which you grant when prompted by your device). You can withdraw consent at
      any time through your device settings.
    </p>

    <h2>Third parties</h2>
    <p>
      We do not sell, rent, or trade your data. We use an anonymised analytics service to collect
      aggregated usage statistics; no personal data is shared with them. The app is distributed
      through the Apple App Store and Google Play Store, which have their own privacy policies.
    </p>

    <h2>How long we keep data</h2>
    <p>
      Anonymised usage data is retained for a maximum of 12 months and then deleted. Location and
      camera data are never stored in the first place, so there is nothing to retain.
    </p>

    <h2>Your rights</h2>
    <p>
      Under the GDPR, you have the right to access, correct, or delete the personal data we hold
      about you, to restrict or object to processing, and to data portability. Because we collect
      minimal data and do not link it to your identity, some of these rights will apply only in
      limited circumstances — we will let you know if that is the case. To exercise any of these
      rights, contact us at <a href="mailto:info@koproductions.nl">info@koproductions.nl</a>. You
      also have the right to lodge a complaint with the Dutch Data Protection Authority at
      <a href="https://autoriteitpersoonsgegevens.nl" target="_blank" rel="noopener">autoriteitpersoonsgegevens.nl</a>.
    </p>

    <h2>Changes</h2>
    <p>
      We may update this policy from time to time. The current version is always available in the
      app. We will notify users of significant changes through the app where technically
      possible.
    </p>

    <h2>Questions?</h2>
    <p>
      K.O. Productions ·
      <a href="mailto:info@koproductions.nl">info@koproductions.nl</a> ·
      <a href="https://koproductions.nl" target="_blank" rel="noopener">koproductions.nl</a>
    </p>
  </main>
</template>

<style scoped>
.privacy {
  max-width: 42rem;
  margin: 0 auto;
  padding: 2.5rem 1.5rem 4rem;
  box-sizing: border-box;
  line-height: 1.6;
}

h1 {
  margin: 1.5rem 0 0.25rem;
  font-size: clamp(1.75rem, 6vw, 2.25rem);
  line-height: 1.2;
}

h2 {
  margin: 2.25rem 0 0.5rem;
  font-size: 1.2rem;
}

p {
  margin: 0 0 1rem;
  color: rgb(245 245 245 / 0.85);
}

.updated {
  color: rgb(245 245 245 / 0.6);
  font-size: 0.9rem;
}

a {
  color: #f5f5f5;
  text-underline-offset: 0.15em;
}

.back {
  color: rgb(245 245 245 / 0.6);
  font-size: 0.9rem;
  text-decoration: none;
}

.back:hover,
.back:focus-visible {
  color: #f5f5f5;
}
</style>
