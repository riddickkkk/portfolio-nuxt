<script setup lang="ts">
// SEO Composables required by Professor Sylvan Cahilog
useHead({
  title: 'Rean Riddick Guinto | Portfolio',
  meta: [
    { name: 'description', content: 'Portfolio of Rean Riddick Garcia Guinto - Front-End Web Developer.' }
  ]
})

useSeoMeta({
  title: 'Rean Riddick Guinto - Portfolio',
  ogTitle: 'Rean Riddick Guinto - Portfolio',
  description: 'IT Student & Front-End Web Developer',
  ogDescription: 'IT Student & Front-End Web Developer'
})
</script>

<template>
  <div class="min-h-screen bg-gradient-to-b from-[#182615] via-[#1f331b] to-[#142111] text-[#fdfbf7] font-sans flex flex-col justify-between">
    <!-- Navbar Header Component -->
    <AppHeader />

    <!-- Hero Section (Centered) -->
    <main class="flex-1 flex flex-col items-center justify-center text-center px-4 py-12">
      <!-- Circular Glowing Profile Image -->
      <div class="relative mb-6">
        <div class="w-36 h-36 rounded-full overflow-hidden border-4 border-[#527346] shadow-[0_0_30px_rgba(163,177,138,0.3)] bg-[#2a3a24] mx-auto flex items-center justify-center">
          <!-- Uses your picture from public/rean.png -->
          <img 
            src="/rean.png" 
            alt="Rean Riddick Guinto" 
            class="w-full h-full object-cover"
          />
        </div>
      </div>

      <!-- Full Name -->
      <h1 class="text-3xl md:text-4xl font-bold tracking-tight text-[#fdfbf7] mb-2">
        Rean Riddick Guinto
      </h1>

      <!-- Role / Subtitle -->
      <p class="text-xs md:text-sm font-semibold tracking-widest text-[#a3b18a] uppercase mb-6">
        FRONT-END WEB DEVELOPER & IT STUDENT
      </p>

      <!-- Center Rounded Card / Bio -->
      <div class="max-w-xl w-full bg-[#1b2b18]/80 backdrop-blur-md border border-[#3f5a36]/50 rounded-2xl p-6 mb-8 shadow-lg">
        <p class="text-sm md:text-base text-[#dad7cd] leading-relaxed">
          Building responsive, modern web applications and dedicated to creating clean, user-focused digital experiences.
        </p>
      </div>

      <!-- Lower Action Pills -->
      <div class="flex flex-wrap justify-center gap-3">
        <a href="#about" class="px-6 py-2.5 bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all shadow-md">
          ABOUT ME
        </a>
        <a href="#certificates" class="px-6 py-2.5 bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all shadow-md">
          CERTIFICATES
        </a>
        <a href="#techstack" class="px-6 py-2.5 bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all shadow-md">
          TECH STACK
        </a>
        <a href="#contacts" class="px-6 py-2.5 bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all shadow-md">
          CONTACTS
        </a>
      </div>
    </main>

    <!-- Empty footer space to maintain vertical balance -->
    <footer class="py-6"></footer>
  </div>
</template>