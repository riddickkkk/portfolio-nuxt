<script setup lang="ts">
import { Wrench } from 'lucide-vue-next'

const techItems = [
  { name: 'C', icon: '/pictures/cproglogo.png' },
  { name: 'Java', icon: '/pictures/javalogo.png' },
  { name: 'HTML', icon: '/pictures/htmllogo.png' },
  { name: 'CSS', icon: '/pictures/csslogo.png' },
  { name: 'MySQL', icon: '/pictures/mysql-white-icon.png' },
  { name: 'Android Studio', icon: '/pictures/androidstudio-logo.png' },
  { name: 'VS Code', icon: '/pictures/vscodelogo.png' },
  { name: 'GitHub', icon: '/pictures/white.png' },
  { name: 'Git', icon: '/pictures/gitlogo.png' },
  { name: 'JavaScript', icon: '/pictures/javascriptlogo.png' }
]
</script>

<template>
  <section id="techstack" class="py-16 px-4">
    <div class="max-w-4xl mx-auto">
      <!-- Section Title & Subtitle -->
      <div class="flex flex-col items-center justify-center mb-10 text-center">
        <div class="flex items-center gap-2 mb-2">
          <Wrench class="w-6 h-6 text-[#a3b18a]" />
          <h2 class="text-3xl font-bold text-[#fdfbf7]">TECH STACK</h2>
        </div>
        <p class="text-sm text-[#a3b18a]">
          Here are my programming languages and tools that I'm familiar with:
        </p>
      </div>

      <!-- Tech Grid -->
      <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-5 gap-4">
        <div 
          v-for="(tech, index) in techItems" 
          :key="index"
          class="flex flex-col items-center justify-center p-5 bg-[#1b2b18]/80 border border-[#3f5a36]/50 rounded-2xl shadow-lg hover:border-[#5e8350] hover:bg-[#1b2b18] transition-all group"
        >
          <div class="w-12 h-12 flex items-center justify-center mb-3">
            <img 
              :src="tech.icon" 
              :alt="tech.name" 
              class="max-h-full max-w-full object-contain group-hover:scale-110 transition-transform"
            />
          </div>
          <span class="text-xs font-semibold text-[#fdfbf7] tracking-wide text-center">
            {{ tech.name }}
          </span>
        </div>
      </div>
    </div>
  </section>
</template>