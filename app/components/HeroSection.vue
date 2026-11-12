<script setup lang="ts">
import { User, Award, Wrench, Mail } from 'lucide-vue-next'

// 1. Page-level SEO setup
useHead({
  title: 'Rean Riddick Guinto | Aspiring Cybersecurity Specialist'
})

useSeoMeta({
  title: 'Rean Riddick Guinto | Aspiring Cybersecurity Specialist',
  ogTitle: 'Rean Riddick Guinto | Aspiring Cybersecurity Specialist',
  description: 'Personal portfolio of Rean Riddick Garcia Guinto — an Information Technology student and aspiring cybersecurity specialist dedicated to securing the tech world.',
  ogDescription: 'Personal portfolio of Rean Riddick Garcia Guinto — an Information Technology student and aspiring cybersecurity specialist dedicated to securing the tech world.',
  twitterCard: 'summary_large_image'
})

// 2. Data-driven navigation buttons
const quickLinks = [
  { label: 'ABOUT ME', to: '/about', icon: User },
  { label: 'CERTIFICATES', to: '/certificates', icon: Award },
  { label: 'TECH STACK', to: '/tech-stack', icon: Wrench },
  { label: 'CONTACTS', to: '/contacts', icon: Mail }
]
</script>

<template>
  <section class="hero min-h-screen pt-24 pb-16 px-4 bg-[#182615]">
    <div class="hero-content text-center flex-col max-w-3xl mx-auto">
      <!-- Profile Avatar (DaisyUI) -->
      <div class="avatar mb-4">
        <div class="w-36 md:w-44 rounded-full ring ring-[#5e8350] ring-offset-4 ring-offset-[#182615] shadow-2xl bg-[#253821]">
          <img 
            src="/pictures/Guinto, Rean Riddick G. (1).png" 
            alt="Rean Riddick Guinto" 
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

      <!-- Description Card (DaisyUI) -->
      <div class="card bg-[#1b2b18]/80 border border-[#3f5a36]/50 mb-8 max-w-lg shadow-lg">
        <div class="card-body p-5 md:p-6">
          <p class="text-sm md:text-base text-[#dad7cd] leading-relaxed">
            My dream is working in cybersecurity jobs to ensure safety in the tech world.
          </p>
        </div>
      </div>

      <!-- Section Navigation Buttons -->
      <div class="flex flex-wrap items-center justify-center gap-3">
        <NuxtLink 
          v-for="link in quickLinks"
          :key="link.to"
          :to="link.to" 
          class="btn bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full px-5 text-xs tracking-wider transition-all shadow-md flex items-center gap-2"
        >
          <component :is="link.icon" class="w-4 h-4" />
          {{ link.label }}
        </NuxtLink>
      </div>
    </div>
  </section>
</template>