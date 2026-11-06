<template>
  <header class="fixed top-0 left-0 w-full z-50 bg-[#182615]/90 backdrop-blur-md border-b border-[#3f5a36]/30 px-6 py-4 flex items-center justify-between">
    <NuxtLink to="/" class="text-lg font-bold text-[#fdfbf7] bg-[#4f6f43] px-4 py-1.5 rounded-full shadow-sm">
      Rean Riddick
    </NuxtLink>

    <nav class="hidden md:flex items-center gap-2">
      <NuxtLink 
        to="/" 
        class="btn btn-ghost text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-full"
        active-class="bg-[#4f6f43] text-[#fdfbf7]"
      >
        HOME
      </NuxtLink>
      <NuxtLink 
        to="/about" 
        class="btn btn-ghost text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-full"
        active-class="bg-[#4f6f43] text-[#fdfbf7]"
      >
        ABOUT ME
      </NuxtLink>
      <NuxtLink 
        to="/certificates" 
        class="btn btn-ghost text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-full"
        active-class="bg-[#4f6f43] text-[#fdfbf7]"
      >
        CERTIFICATES
      </NuxtLink>
      <NuxtLink 
        to="/tech-stack" 
        class="btn btn-ghost text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-full"
        active-class="bg-[#4f6f43] text-[#fdfbf7]"
      >
        TECH STACK
      </NuxtLink>
      <NuxtLink 
        to="/contacts" 
        class="btn btn-ghost text-xs text-[#dad7cd] hover:text-[#fdfbf7] hover:bg-[#253821] rounded-full"
        active-class="bg-[#4f6f43] text-[#fdfbf7]"
      >
        CONTACTS
      </NuxtLink>
    </nav>
  </header>
</template>