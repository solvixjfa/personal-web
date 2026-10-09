<script setup>
import { store } from '../store.js'
</script>

<template>
  <section id="hero" class="max-w-5xl mx-auto px-6 py-28 text-center flex flex-col items-center justify-center min-h-[80vh]">
    <div class="inline-block px-4 py-1.5 mb-8 rounded-full border border-white/10 bg-white/5 text-gray-300 text-xs font-medium tracking-widest uppercase backdrop-blur-sm">
      AI Engineer & Fullstack Developer
    </div>
    
    <h1 class="text-5xl sm:text-7xl font-extrabold text-white tracking-tight mb-6 leading-none">
      Jeffry
    </h1>
    
    <p v-if="store.lang === 'en'" class="text-base sm:text-xl text-gray-400 max-w-2xl mx-auto mb-10 leading-relaxed font-light">
      I build smart systems and AI agents that actually work in production. From designing backend architectures to deploying autonomous business logic.
    </p>
    <p v-else class="text-base sm:text-xl text-gray-400 max-w-2xl mx-auto mb-10 leading-relaxed font-light">
      Saya merancang dan membangun sistem AI yang siap berjalan di production. Mulai dari arsitektur backend hingga eksekusi logika bisnis otonom.
    </p>

    <div class="flex flex-col sm:flex-row gap-4 w-full sm:w-auto">
      <a href="#contact" class="px-8 py-3.5 bg-white text-black font-bold text-xs tracking-widest uppercase rounded transition-all hover:bg-gray-200 shadow-lg flex items-center justify-center gap-2">
        <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
        {{ store.lang === 'en' ? 'Get In Touch' : 'Hubungi Saya' }}
      </a>
      <a href="https://drive.google.com/file/d/1pcx5h3UhlQL-XCukDZ4WF-fMv7SQ9RKu/view?usp=drivesdk" target="_blank" class="px-8 py-3.5 glossy-card text-white font-bold text-xs tracking-widest uppercase rounded transition-all hover:bg-white/10 flex items-center justify-center gap-2">
        <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4"></path></svg>
        {{ store.lang === 'en' ? 'Download Resume' : 'Unduh CV' }}
      </a>
    </div>
  </section>
</template>
