<script setup lang="ts">
import { ref } from 'vue'
import { Award, ExternalLink, X } from 'lucide-vue-next'

const certificates = [
  {
    title: 'IT Java Specialist',
    image: '/pictures/java.png',
    credlyUrl: 'https://www.credly.com/badges/6a908120-d935-4c2f-8c88-5656b47a01f1'
  },
  {
    title: 'Microsoft PowerPoint Specialist',
    image: '/pictures/point.png',
    credlyUrl: 'https://www.credly.com/badges/07a38bea-7abb-4569-b013-623c0cc60a30'
  }
]

// Lightbox modal state
const activeImage = ref<string | null>(null)

const openLightbox = (imagePath: string) => {
  activeImage.value = imagePath
}

const closeLightbox = () => {
  activeImage.value = null
}
</script>

<template>
  <section id="certificates" class="py-16 px-4 bg-[#142111]/40">
    <div class="max-w-5xl mx-auto">
      <!-- Section Title -->
      <div class="flex items-center justify-center gap-2 mb-8">
        <Award class="w-6 h-6 text-[#a3b18a]" />
        <h2 class="text-3xl font-bold text-center text-[#fdfbf7]">My Certificates</h2>
      </div>

      <!-- Certificates Grid -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div 
          v-for="(cert, index) in certificates" 
          :key="index"
          class="card bg-[#1b2b18]/80 border border-[#3f5a36]/50 overflow-hidden shadow-lg hover:border-[#5e8350] transition-all flex flex-col justify-between"
        >
          <!-- Certificate Image (Clickable for Lightbox) -->
          <figure class="px-4 pt-4 cursor-pointer" @click="openLightbox(cert.image)">
            <img 
              :src="cert.image" 
              :alt="cert.title" 
              class="rounded-xl h-56 w-full object-cover border border-[#3f5a36]/30 hover:opacity-90 transition-opacity"
            />
          </figure>

          <!-- Card Body -->
          <div class="card-body p-5 flex flex-row items-center justify-between">
            <h3 class="card-title text-base text-[#fdfbf7]">{{ cert.title }}</h3>
            <a 
              :href="cert.credlyUrl" 
              target="_blank" 
              class="btn btn-sm bg-[#4f6f43] hover:bg-[#5e8350] text-[#fdfbf7] border-none rounded-full text-xs font-bold uppercase flex items-center gap-1 shrink-0"
            >
              VIEW <ExternalLink class="w-3.5 h-3.5" />
            </a>
          </div>
        </div>
      </div>
    </div>

    <!-- Vue Lightbox Modal -->
    <div 
      v-if="activeImage" 
      class="fixed inset-0 z-50 bg-black/80 backdrop-blur-sm flex items-center justify-center p-4"
      @click.self="closeLightbox"
    >
      <div class="relative max-w-4xl w-full flex flex-col items-center">
        <button 
          @click="closeLightbox" 
          class="absolute -top-10 right-0 text-[#fdfbf7] hover:text-[#a3b18a] p-2"
        >
          <X class="w-8 h-8" />
        </button>
        <img 
          :src="activeImage" 
          alt="Certificate Full View" 
          class="max-h-[85vh] w-auto rounded-lg border border-[#3f5a36]/50 shadow-2xl object-contain"
        />
      </div>
    </div>
  </section>
</template>