<template>
  <section id="contact" class="py-20 border-t border-white/5 bg-[#080808]">
    <div class="max-w-4xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-xs font-bold tracking-[0.3em] text-gray-400 uppercase mb-3">INITIATE A SYSTEM</h2>
        <p class="text-2xl sm:text-3xl font-bold text-white">Ready to deploy high-ticket business automation?</p>
      </div>

      <div class="grid sm:grid-cols-3 gap-6 mb-12">
        <a href="mailto:Jeffry4job@gmail.com" class="glossy-card p-6 rounded-xl flex items-center gap-4 group">
          <div class="w-10 h-10 rounded-full border border-white/20 bg-white/5 flex items-center justify-center text-white">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
          </div>
          <div>
            <div class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">EMAIL</div>
            <div class="text-xs font-semibold text-white truncate">Jeffry4job@gmail.com</div>
          </div>
        </a>

        <a href="https://wa.me/6285736048626" target="_blank" class="glossy-card p-6 rounded-xl flex items-center gap-4 group">
          <div class="w-10 h-10 rounded-full border border-white/20 bg-white/5 flex items-center justify-center text-white">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z"></path></svg>
          </div>
          <div>
            <div class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">WHATSAPP</div>
            <div class="text-xs font-semibold text-white">+62 857-3604-8626</div>
          </div>
        </a>

        <div class="glossy-card p-6 rounded-xl flex items-center gap-4">
          <div class="w-10 h-10 rounded-full border border-white/20 bg-white/5 flex items-center justify-center text-white">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
          </div>
          <div>
            <div class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">LOCATION</div>
            <div class="text-xs font-semibold text-white">East Java, Indonesia</div>
          </div>
        </div>
      </div>

      <!-- Formspree Integration -->
      <div class="glossy-card p-8 rounded-2xl max-w-2xl mx-auto">
        <form action="https://formspree.io/f/mldnpnaq" method="POST" class="space-y-6">
          <div class="grid sm:grid-cols-2 gap-6">
            <div>
              <label class="block text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-2">YOUR NAME</label>
              <input type="text" name="name" required class="w-full bg-[#050505] border border-white/10 rounded px-4 py-3 text-sm text-white focus:outline-none focus:border-white/40 transition-colors" placeholder="John Doe" />
            </div>
            <div>
              <label class="block text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-2">YOUR EMAIL</label>
              <input type="email" name="email" required class="w-full bg-[#050505] border border-white/10 rounded px-4 py-3 text-sm text-white focus:outline-none focus:border-white/40 transition-colors" placeholder="john@example.com" />
            </div>
          </div>
          <div>
            <label class="block text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-2">SYSTEM REQUIREMENT</label>
            <textarea name="message" rows="4" required class="w-full bg-[#050505] border border-white/10 rounded px-4 py-3 text-sm text-white focus:outline-none focus:border-white/40 transition-colors" placeholder="Describe project or automation needs..."></textarea>
          </div>
          <button type="submit" class="w-full py-4 bg-white text-black font-bold text-xs tracking-widest uppercase rounded hover:bg-gray-200 transition-colors">
            TRANSMIT
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
