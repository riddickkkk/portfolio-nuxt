<script setup lang="ts">
useHead({
  title: 'Rean Riddick Guinto | Portfolio',
  link: [
    { rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }
  ]
})

useSeoMeta({
  title: 'Rean Riddick Guinto | Portfolio',
  ogTitle: 'Rean Riddick Guinto | Portfolio',
  description: 'Personal portfolio of Rean Riddick Garcia Guinto built with Nuxt 4, Tailwind CSS, and DaisyUI.',
  ogDescription: 'Personal portfolio of Rean Riddick Garcia Guinto built with Nuxt 4, Tailwind CSS, and DaisyUI.',
  ogImage: '/pictures/Guinto, Rean Riddick G. (1).png',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <div class="min-h-screen flex flex-col bg-[#182615] text-[#fdfbf7] font-sans antialiased selection:bg-[#4f6f43] selection:text-[#fdfbf7]">
    <AppHeader />
    <main class="flex-grow">
      <NuxtPage />
    </main>
    <FooterSection />
  </div>
</template>