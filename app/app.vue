<script setup lang="ts">
useHead({
  title: 'Rean Riddick Guinto | Portfolio',
  meta: [
    { name: 'description', content: 'Personal portfolio of Rean Riddick Garcia Guinto built with Nuxt 4, Tailwind CSS, and DaisyUI.' }
  ],
  link: [
    { rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }
  ]
})
</script>

<template>
  <div class="min-h-screen bg-[#182615] text-[#fdfbf7] font-sans antialiased selection:bg-[#4f6f43] selection:text-[#fdfbf7]">
    <!-- Sticky Navigation Bar -->
    <AppHeader />

    <main>
      <!-- Hero / Landing Section -->
      <HeroSection />

      <!-- About Me Section -->
      <AboutSection />

      <!-- Certificates Section -->
      <CertificatesSection />

      <!-- Tech Stack Section -->
      <TechStackSection />

      <!-- Contact Section -->
      <ContactSection />
    </main>

    <!-- Footer -->
    <FooterSection />
  </div>
</template>

<style>
html {
  scroll-behavior: smooth;
}
</style>