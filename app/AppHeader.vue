<template>
  <header class="w-full px-8 py-6 flex justify-between items-center max-w-7xl mx-auto">
    <!-- Left Logo Pill -->
    <NuxtLink 
      to="/" 
      class="px-5 py-2 bg-[#2d4027] hover:bg-[#3a5232] text-[#fdfbf7] rounded-full text-sm font-semibold transition-all border border-[#3f5737]/40 shadow-sm"
    >
      Rean Riddick
    </NuxtLink>

    <!-- Right Navigation Pills -->
    <nav class="flex items-center gap-3">
      <a href="#home" class="px-5 py-2 bg-[#425938] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all shadow-sm">
        HOME
      </a>
      <a href="#about" class="px-5 py-2 bg-[#2d4027] hover:bg-[#3a5232] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all border border-[#3f5737]/40">
        ABOUT ME
      </a>
      <a href="#certificates" class="px-5 py-2 bg-[#2d4027] hover:bg-[#3a5232] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all border border-[#3f5737]/40">
        CERTIFICATES
      </a>
      <a href="#techstack" class="px-5 py-2 bg-[#2d4027] hover:bg-[#3a5232] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all border border-[#3f5737]/40">
        TECH STACK
      </a>
      <a href="#contacts" class="px-5 py-2 bg-[#2d4027] hover:bg-[#3a5232] text-[#fdfbf7] rounded-full text-xs font-bold tracking-wider uppercase transition-all border border-[#3f5737]/40">
        CONTACTS
      </a>
    </nav>
  </header>
</template>