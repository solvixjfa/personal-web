<script setup>
import { store } from '../store.js'
</script>

<template>
  <section id="contact" class="py-20 border-t border-white/5 bg-[#050505]">
    <div class="max-w-4xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-[10px] font-mono tracking-[0.3em] text-gray-500 uppercase mb-3">
          {{ store.lang === 'en' ? 'Initiate a System' : 'Ayo Berkolaborasi' }}
        </h2>
        <p class="text-2xl sm:text-3xl font-bold text-white">
          {{ store.lang === 'en' ? "Let's build something cool." : 'Mari diskusi soal proyekmu.' }}
        </p>
        <p class="text-sm text-gray-400 mt-4">
          {{ store.lang === 'en' ? 'Got a business problem that needs automating? Drop me a line.' : 'Ada masalah bisnis yang pengen di-otomatisasi? Hubungi saya aja.' }}
        </p>
      </div>

      <div class="grid sm:grid-cols-2 gap-6 mb-16">
        <a href="mailto:Jeffry4job@gmail.com" class="border border-white/10 p-6 rounded-xl flex items-center justify-center gap-4 hover:bg-white/5 transition-colors">
          <div class="text-[10px] font-mono tracking-widest text-gray-500 uppercase">EMAIL</div>
          <div class="text-sm font-bold text-white truncate">Jeffry4job@gmail.com</div>
        </a>

        <a href="https://wa.me/6285736048626" target="_blank" class="border border-white/10 p-6 rounded-xl flex items-center justify-center gap-4 hover:bg-white/5 transition-colors">
          <div class="text-[10px] font-mono tracking-widest text-gray-500 uppercase">WHATSAPP</div>
          <div class="text-sm font-bold text-white">+62 857-3604-8626</div>
        </a>
      </div>

      <!-- Formspree Integration -->
      <div class="border border-white/10 bg-[#0a0a0a] p-8 rounded-2xl max-w-2xl mx-auto">
        <form action="https://formspree.io/f/mldnpnaq" method="POST" class="space-y-6">
          <div class="grid sm:grid-cols-2 gap-6">
            <div>
              <label class="block text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-2">
                {{ store.lang === 'en' ? 'Your Name' : 'Nama Kamu' }}
              </label>
              <input type="text" name="name" required class="w-full bg-transparent border-b border-white/20 px-0 py-3 text-sm text-white focus:outline-none focus:border-white transition-colors" :placeholder="store.lang === 'en' ? 'John Doe' : 'Budi Santoso'" />
            </div>
            <div>
              <label class="block text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-2">
                {{ store.lang === 'en' ? 'Your Email' : 'Email Kamu' }}
              </label>
              <input type="email" name="email" required class="w-full bg-transparent border-b border-white/20 px-0 py-3 text-sm text-white focus:outline-none focus:border-white transition-colors" placeholder="email@example.com" />
            </div>
          </div>
          <div>
            <label class="block text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-2">
              {{ store.lang === 'en' ? 'Tell me about the project' : 'Ceritain kebutuhan sistemmu' }}
            </label>
            <textarea name="message" rows="3" required class="w-full bg-transparent border-b border-white/20 px-0 py-3 text-sm text-white focus:outline-none focus:border-white transition-colors" :placeholder="store.lang === 'en' ? 'I need an AI system that...' : 'Saya butuh otomatisasi buat...'"></textarea>
          </div>
          <button type="submit" class="w-full py-4 bg-white text-black font-bold text-xs tracking-widest uppercase rounded hover:bg-gray-200 transition-colors mt-4">
            {{ store.lang === 'en' ? 'Send Message' : 'Kirim Pesan' }}
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
