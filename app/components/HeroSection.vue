<script setup lang="ts">
import { User, Award, Wrench, Mail } from 'lucide-vue-next'
</script>

<template>
  <section id="home" class="min-h-screen flex items-center justify-center pt-24 pb-16 px-4 bg-[#182615]">
    <div class="max-w-3xl mx-auto text-center flex flex-col items-center">
      <!-- Profile Image -->
      <div class="relative mb-6">
        <div class="w-36 h-36 md:w-44 md:h-44 rounded-full overflow-hidden border-4 border-[#5e8350] shadow-2xl bg-[#253821]">
          <img 
           src="/pictures/Guinto, Rean Riddick G. (1).png" 
           alt="Rean Riddick Guinto" 
           class="w-full h-full object-cover"
          />
        </div>
      </div>

      <!-- Name & Title -->
      <h1 class="text-3xl md:text-5xl font-extrabold text-[#fdfbf7] tracking-tight mb-2">
        Rean Riddick Guinto
      </h1>
      
      <p class="text-xs md:text-sm uppercase tracking-widest text-[#a3b18a] font-semibold mb-6">
        ASPIRING CYBERSECURITY SPECIALIST
      </p>

      <!-- Description Box -->
      <div class="bg-[#1b2b18]/80 border border-[#3f5a36]/50 rounded-2xl p-5 md:p-6 mb-8 max-w-lg shadow-lg">
        <p class="text-sm md:text-base text-[#dad7cd] leading-relaxed">
          My dream is working in cybersecurity jobs to ensure safety in the tech world.
        </p>
      </div>

      <!-- Original Section Pill Buttons -->
      <div class="flex flex-wrap items-center justify-center gap-3">
        <a 
          href="#about" 
          class="btn bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full px-5 text-xs tracking-wider transition-all shadow-md flex items-center gap-2"
        >
          <User class="w-4 h-4" /> ABOUT ME
        </a>
        <a 
          href="#certificates" 
          class="btn bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full px-5 text-xs tracking-wider transition-all shadow-md flex items-center gap-2"
        >
          <Award class="w-4 h-4" /> CERTIFICATES
        </a>
        <a 
          href="#techstack" 
          class="btn bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full px-5 text-xs tracking-wider transition-all shadow-md flex items-center gap-2"
        >
          <Wrench class="w-4 h-4" /> TECH STACK
        </a>
        <a 
          href="#contacts" 
          class="btn bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full px-5 text-xs tracking-wider transition-all shadow-md flex items-center gap-2"
        >
          <Mail class="w-4 h-4" /> CONTACTS
        </a>
      </div>
    </div>
  </section>
</template>