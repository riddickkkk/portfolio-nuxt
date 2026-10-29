<template>
  <div class="min-h-screen bg-[#1c2419] text-[#fdfbf7] font-sans">
    <!-- Header / Navbar -->
    <header class="border-b border-[#3b4a37] px-8 py-6 flex justify-between items-center max-w-6xl mx-auto">
      <h1 class="text-xl font-bold tracking-wide text-[#a3b18a]">Rean Riddick Guinto</h1>
      <nav class="space-x-6 text-sm font-medium">
        <a href="#about" class="hover:text-[#a3b18a] transition-colors">About</a>
        <a href="#projects" class="hover:text-[#a3b18a] transition-colors">Projects</a>
        <a href="#contact" class="hover:text-[#a3b18a] transition-colors">Contact</a>
      </nav>
    </header>

    <!-- Hero Section -->
    <main class="max-w-4xl mx-auto px-6 py-20 text-center">
      <span class="inline-block px-3 py-1 bg-[#2a3826] text-[#a3b18a] rounded-full text-xs font-semibold mb-4 border border-[#3b4a37]">
        IT Student & Front-End Web Developer
      </span>
      <h2 class="text-4xl md:text-5xl font-extrabold mb-6 text-[#fdfbf7]">
        Building Modern & Responsive Web Applications
      </h2>
      <p class="text-base md:text-lg text-[#cbd5e1] max-w-2xl mx-auto mb-8">
        Welcome to my portfolio! Built with Nuxt 4 and deployed on Render as a Web Service.
      </p>
      <div class="flex justify-center gap-4">
        <a href="#projects" class="bg-[#588157] hover:bg-[#3a5a40] text-[#fdfbf7] px-6 py-3 rounded-lg font-semibold transition-all shadow-md">
          View Projects
        </a>
        <a href="https://github.com/riddickkkk" target="_blank" class="border border-[#3b4a37] hover:bg-[#2a3826] text-[#fdfbf7] px-6 py-3 rounded-lg font-semibold transition-all">
          GitHub Profile
        </a>
      </div>
    </main>
  </div>
</template>

<script setup>
useHead({
  title: 'Rean Riddick Guinto | Portfolio',
  meta: [
    { name: 'description', content: 'Personal Web Development Portfolio built with Nuxt 4' }
  ]
})
</script>