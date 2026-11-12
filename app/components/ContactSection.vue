<script setup lang="ts">
import { Mail } from 'lucide-vue-next'

// 1. Page-level SEO setup
useHead({
  title: 'Contact Me | Rean Riddick Garcia Guinto'
})

useSeoMeta({
  title: 'Contact Me | Rean Riddick Garcia Guinto',
  ogTitle: 'Contact Me | Rean Riddick Garcia Guinto',
  description: 'Get in touch with Rean Riddick Garcia Guinto via GitHub or LinkedIn for software development collaborations, projects, and inquiries.',
  ogDescription: 'Get in touch with Rean Riddick Garcia Guinto via GitHub or LinkedIn for software development collaborations, projects, and inquiries.',
  twitterCard: 'summary_large_image'
})

// 2. Data-driven social links
const socialLinks = [
  {
    name: 'GitHub',
    url: 'https://github.com/riddickkkk/portfolio',
    icon: '/pictures/white.png'
  },
  {
    name: 'LinkedIn',
    url: 'https://www.linkedin.com/in/rean-riddick-guinto-7b4596409/',
    icon: '/pictures/LinkedIn_logo_initials.png'
  }
]
</script>

<template>
  <section id="contacts" class="py-24 px-4 bg-[#142111]/40 min-h-screen flex items-center">
    <div class="max-w-3xl mx-auto w-full">
      <!-- Section Title -->
      <div class="flex items-center justify-center gap-2 mb-8">
        <Mail class="w-6 h-6 text-[#a3b18a]" />
        <h2 class="text-3xl font-bold text-center text-[#fdfbf7]">Contact Me</h2>
      </div>

      <!-- DaisyUI Card Container -->
      <div class="card bg-[#1b2b18]/80 border border-[#3f5a36]/50 shadow-xl">
        <div class="card-body items-center text-center p-8">
          <div class="flex items-center justify-center gap-6">
            <a 
              v-for="social in socialLinks"
              :key="social.name"
              :href="social.url" 
              target="_blank" 
              rel="noopener noreferrer"
              :aria-label="social.name"
              class="btn w-20 h-20 bg-[#253821] hover:bg-[#344d2d] border border-[#3f5a36] hover:border-[#5e8350] rounded-2xl flex items-center justify-center transition-all duration-300 hover:scale-105 shadow-md group p-0"
            >
              <img 
                :src="social.icon" 
                :alt="social.name" 
                class="w-10 h-10 object-contain opacity-90 group-hover:opacity-100"
              />
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>