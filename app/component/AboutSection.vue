<script setup lang="ts">
import { User, Heart, Compass } from 'lucide-vue-next'
</script>

<template>
  <section id="about" class="py-16 px-4">
    <div class="max-w-4xl mx-auto">
      <!-- Section Title -->
      <div class="flex items-center justify-center gap-2 mb-8">
        <User class="w-6 h-6 text-[#a3b18a]" />
        <h2 class="text-3xl font-bold text-center text-[#fdfbf7]">About Me</h2>
      </div>

      
      <div class="space-y-6">
        
        <div class="card bg-[#1b2b18]/80 backdrop-blur-md border border-[#3f5a36]/50 shadow-xl p-6 md:p-8 rounded-2xl text-[#dad7cd]">
          <div class="flex items-start gap-4">
            <div class="p-3 bg-[#4f6f43]/30 border border-[#5e8350]/40 rounded-xl text-[#a3b18a] shrink-0">
              <Compass class="w-6 h-6" />
            </div>
            <div>
              <p class="text-sm md:text-base leading-relaxed text-[#dad7cd]">
                Hi, I’m Rean, a sporty and adventurous person who enjoys staying active and trying new experiences. I love playing sports because they help me stay healthy, disciplined, and focused. I am also a fitness enthusiast who enjoys working out and maintaining a healthy lifestyle. Overall, I aim to grow every day by staying active, curious, and open to challenges.
              </p>
            </div>
          </div>
        </div> 
        <div class="card bg-[#1b2b18]/80 backdrop-blur-md border border-[#3f5a36]/50 shadow-xl p-6 md:p-8 rounded-2xl text-[#dad7cd]">
          <div class="flex items-start gap-4">
            <div class="p-3 bg-[#4f6f43]/30 border border-[#5e8350]/40 rounded-xl text-[#a3b18a] shrink-0">
              <Heart class="w-6 h-6" />
            </div>
            <div>
              <p class="text-sm md:text-base leading-relaxed text-[#dad7cd]">
                My goal in life is to be rich not just in money, but in love, kindness, and meaningful experiences. Success for me isn’t only measured by achievements or possessions, but by the happiness I share and the positive impact I leave on the people around me. I strive to live a life filled with purpose, compassion, and balance — where both my heart and mind grow richer every day.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>