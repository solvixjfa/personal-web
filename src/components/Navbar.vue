<script setup>
import { ref, watch } from 'vue'
import { store } from '../store.js'

const isSidebarOpen = ref(false)

watch(isSidebarOpen, (isOpen) => {
  if (isOpen) {
    document.body.style.overflow = 'hidden'
  } else {
    document.body.style.overflow = 'auto'
  }
})

const navLinks = {
  en: [
    { name: 'HOME', href: '#hero' },
    { name: 'ABOUT', href: '#about' },
    { name: 'PROJECTS', href: '#projects' },
    { name: 'EXPERIENCE', href: '#experience' }
  ],
  id: [
    { name: 'BERANDA', href: '#hero' },
    { name: 'TENTANG', href: '#about' },
    { name: 'PROYEK', href: '#projects' },
    { name: 'PENGALAMAN', href: '#experience' }
  ]
}
</script>

<template>
  <header class="border-b border-white/5 sticky top-0 bg-[#050505]/90 backdrop-blur-md z-40">
    <div class="max-w-6xl mx-auto px-6 h-16 flex items-center justify-between">
      <a href="#hero" class="font-bold text-xl tracking-widest text-white">Jeffry</a>

      <!-- PC Nav -->
      <nav class="hidden md:flex gap-8 items-center">
        <a v-for="link in navLinks[store.lang]" :key="link.name" :href="link.href" class="text-xs tracking-widest font-semibold text-gray-400 hover:text-white transition-colors">
          {{ link.name }}
        </a>
        <button @click="store.lang = store.lang === 'en' ? 'id' : 'en'" class="ml-4 px-3 py-1 rounded-full border border-white/20 text-xs font-bold text-white hover:bg-white hover:text-black transition-colors flex items-center gap-2">
          <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5h12M9 3v2m1.048 9.5A18.022 18.022 0 016.412 9m6.088 9h7M11 21l5-10 5 10M12.751 5C11.783 10.77 8.07 15.61 3 18.129"></path></svg>
          {{ store.lang === 'en' ? 'ID' : 'EN' }}
        </button>
      </nav>

      <!-- Mobile Hamburger & Lang Toggle -->
      <div class="flex items-center gap-4 md:hidden">
        <button @click="store.lang = store.lang === 'en' ? 'id' : 'en'" class="text-xs font-bold text-gray-400 hover:text-white border border-white/20 px-2 py-1 rounded">
          {{ store.lang === 'en' ? 'ID' : 'EN' }}
        </button>
        <button @click="isSidebarOpen = true" class="p-2 text-gray-400 hover:text-white focus:outline-none">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
        </button>
      </div>
    </div>

    <!-- Mobile Drawer -->
    <Teleport to="body">
      <div v-if="isSidebarOpen" class="fixed inset-0 bg-black/80 z-[999] md:hidden" @click="isSidebarOpen = false"></div>
      <div class="fixed top-0 right-0 h-[100dvh] w-4/5 max-w-sm bg-[#0a0a0a] border-l border-white/10 z-[1000] p-6 shadow-2xl transition-transform duration-300 md:hidden flex flex-col justify-between" :class="isSidebarOpen ? 'translate-x-0' : 'translate-x-full'">
        <div>
          <div class="flex justify-between items-center pb-4 border-b border-white/10 mb-6">
            <span class="font-bold text-sm tracking-widest text-white">MENU</span>
            <button @click="isSidebarOpen = false" class="p-2 text-gray-400 hover:text-white">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path></svg>
            </button>
          </div>
          <nav class="flex flex-col gap-5">
            <a v-for="link in navLinks[store.lang]" :key="link.name" :href="link.href" @click="isSidebarOpen = false" class="text-sm font-semibold tracking-widest text-gray-300 hover:text-white py-2 border-b border-white/5">
              {{ link.name }}
            </a>
          </nav>
        </div>
      </div>
    </Teleport>
  </header>
</template>
