<script setup lang="ts">
const navLinks = [
  { label: 'HOME', to: '/' },
  { label: 'ABOUT ME', to: '/about' },
  { label: 'CERTIFICATES', to: '/certificates' },
  { label: 'TECH STACK', to: '/tech-stack' },
  { label: 'CONTACTS', to: '/contacts' }
]
</script>

<template>
  <header class="navbar fixed top-0 left-0 w-full z-50 bg-[#182615]/90 backdrop-blur-md border-b border-[#3f5a36]/30 px-6 py-3">
    <!-- Navbar Start: Brand Logo & Mobile Dropdown -->
    <div class="navbar-start">
      <!-- Mobile Menu (DaisyUI Dropdown) -->
      <div class="dropdown md:hidden mr-2">
        <div tabindex="0" role="button" class="btn btn-ghost btn-circle text-[#fdfbf7]">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h7" />
          </svg>
        </div>
        <ul tabindex="0" class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow-xl bg-[#1b2b18] border border-[#3f5a36]/50 rounded-box w-52 space-y-1">
          <li v-for="link in navLinks" :key="link.to">
            <NuxtLink 
              :to="link.to" 
              class="text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-lg"
              active-class="bg-[#4f6f43] text-[#fdfbf7]"
            >
              {{ link.label }}
            </NuxtLink>
          </li>
        </ul>
      </div>

      <!-- Brand Pill -->
      <NuxtLink to="/" class="text-lg font-bold text-[#fdfbf7] bg-[#4f6f43] px-4 py-1.5 rounded-full shadow-sm hover:bg-[#5e8350] transition-colors">
        Rean Riddick
      </NuxtLink>
    </div>

    <!-- Navbar End: Desktop Links -->
    <nav class="navbar-end hidden md:flex">
      <ul class="menu menu-horizontal px-1 gap-2">
        <li v-for="link in navLinks" :key="link.to">
          <NuxtLink 
            :to="link.to" 
            class="btn btn-ghost btn-sm text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-full"
            active-class="bg-[#4f6f43] text-[#fdfbf7]"
          >
            {{ link.label }}
          </NuxtLink>
        </li>
      </ul>
    </nav>
  </header>
</template>