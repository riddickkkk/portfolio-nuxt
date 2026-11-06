<script setup lang="ts">
useHead({
  title: 'Rean Riddick Guinto | Portfolio',
  meta: [
    { name: 'description', content: 'Portfolio of Rean Riddick Garcia Guinto.' }
  ]
})

useSeoMeta({
  title: 'Rean Riddick Guinto - Portfolio',
  ogTitle: 'Rean Riddick Guinto - Portfolio',
  description: 'IT Student',
  ogDescription: 'IT Student'
})
</script>

<template>
  <div class="min-h-screen bg-gradient-to-b from-[#182615] via-[#1f331b] to-[#142111] text-[#fdfbf7] font-sans flex flex-col justify-between">
    <AppHeader />
    <main>
      <HeroSection />
      <AboutSection id="about" />
      <CertificatesSection id="certificates" />
      <TechStackSection id="techstack" />
      <ContactSection id="contacts" />
    </main>
    <FooterSection />
  </div>
</template>