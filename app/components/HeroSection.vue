<script setup lang="ts">
import { Code, Sparkles, MapPin } from 'lucide-vue-next'
</script>

<template>
  <section class="min-h-[80vh] flex flex-col items-center justify-center text-center px-4 py-16 relative">
    <div class="max-w-3xl mx-auto flex flex-col items-center">
      <!-- Profile Picture -->
      <div class="relative mb-6">
        <div class="w-32 h-32 md:w-40 md:h-40 rounded-full overflow-hidden border-4 border-[#5e8350] shadow-2xl">
          <img 
            src="/rean.png" 
            alt="Rean Riddick Guinto" 
            class="w-full h-full object-cover"
          />
        </div>
        <div class="absolute bottom-1 right-1 bg-[#4f6f43] text-[#fdfbf7] p-2 rounded-full border-2 border-[#182615]">
          <Sparkles class="w-4 h-4" />
        </div>
      </div>

      <!-- Badge -->
      <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-[#1b2b18] border border-[#3f5a36] text-[#a3b18a] text-xs font-semibold mb-4">
        <MapPin class="w-3.5 h-3.5" /> Bacoor, Cavite
      </div>

      <!-- Main Title -->
      <h1 class="text-4xl md:text-6xl font-extrabold text-[#fdfbf7] tracking-tight mb-4">
        Rean Riddick Garcia Guinto
      </h1>

      <!-- Subtitle -->
      <p class="text-lg md:text-xl text-[#a3b18a] font-medium max-w-xl mb-6">
        IT Student & Front-End Developer
      </p>

      <!-- Action Buttons -->
      <div class="flex flex-wrap justify-center gap-4">
        <a 
          href="#about" 
          class="btn bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full px-6 text-xs font-bold uppercase tracking-wider shadow-lg transition-all"
        >
          Explore Portfolio
        </a>
        <a 
          href="#contacts" 
          class="btn btn-outline border-[#5e8350] text-[#fdfbf7] hover:bg-[#4f6f43] rounded-full px-6 text-xs font-bold uppercase tracking-wider transition-all"
        >
          Contact Me
        </a>
      </div>
    </div>
  </section>
</template>