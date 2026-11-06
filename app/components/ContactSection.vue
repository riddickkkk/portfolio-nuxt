<script setup lang="ts">
import { Mail } from 'lucide-vue-next'
</script>

<template>
  <section id="contacts" class="py-16 px-4 bg-[#142111]/40">
    <div class="max-w-3xl mx-auto">
      <!-- Section Title -->
      <div class="flex items-center justify-center gap-2 mb-8">
        <Mail class="w-6 h-6 text-[#a3b18a]" />
        <h2 class="text-3xl font-bold text-center text-[#fdfbf7]">Contact Me</h2>
      </div>

      <!-- Social Icons Container -->
      <div class="bg-[#1b2b18]/80 border border-[#3f5a36]/50 rounded-2xl p-8 shadow-xl text-center">
        <div class="flex items-center justify-center gap-6">
          <!-- GitHub Link -->
          <a 
            href="https://github.com/riddickkkk/portfolio" 
            target="_blank" 
            rel="noopener noreferrer"
            class="w-20 h-20 bg-[#253821] hover:bg-[#344d2d] border border-[#3f5a36] rounded-2xl flex items-center justify-center transition-all duration-300 hover:scale-105 shadow-md group"
          >
            <img 
              src="/pictures/white.png" 
              alt="GitHub" 
              class="w-10 h-10 object-contain opacity-90 group-hover:opacity-100"
            />
          </a>

          <!-- LinkedIn Link -->
          <a 
            href="https://www.linkedin.com/in/rean-riddick-guinto-7b4596409/" 
            target="_blank" 
            rel="noopener noreferrer"
            class="w-20 h-20 bg-[#253821] hover:bg-[#344d2d] border border-[#3f5a36] rounded-2xl flex items-center justify-center transition-all duration-300 hover:scale-105 shadow-md group"
          >
            <img 
              src="/pictures/LinkedIn_logo_initials.png" 
              alt="LinkedIn" 
              class="w-10 h-10 object-contain opacity-90 group-hover:opacity-100"
            />
          </a>
        </div>
      </div>
    </div>
  </section>
</template>