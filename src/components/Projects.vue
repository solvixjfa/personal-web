<script setup>
import { store } from '../store.js'
</script>

<template>
  <section id="projects" class="py-20 border-t border-white/5 bg-[#050505]">
    <div class="max-w-5xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-xs font-bold tracking-[0.3em] text-gray-400 uppercase mb-3">
          {{ store.lang === 'en' ? 'Featured Work' : 'Portofolio Utama' }}
        </h2>
        <p class="text-2xl sm:text-3xl font-bold text-white">
          {{ store.lang === 'en' ? 'Selected Projects & Systems' : 'Sistem & Proyek Pilihan' }}
        </p>
      </div>

      <div class="grid md:grid-cols-2 gap-8">
        
        <!-- Project 1: Niki CoC -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-4 block">COMMUNITY SAAS / DISCORD BOT</span>
            <h3 class="text-xl font-bold text-white mb-3">Niki CoC Bot</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              {{ store.lang === 'en' 
                ? 'Autonomous Discord bot for Clash of Clans management. Features real-time war updates, CWL analytics, and AI-powered clan audits.' 
                : 'Bot Discord otonom untuk manajemen Clash of Clans. Dilengkapi fitur update war real-time, analitik CWL, dan audit clan berbasis AI.' }}
            </p>
            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Python</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Discord API</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Gemini</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Vue 3</span>
            </div>
          </div>
          <div class="mt-auto flex justify-center border-t border-white/10 pt-6">
            <a href="https://coc.ixiera.id" target="_blank" class="px-8 py-2.5 border border-white/20 rounded-full text-[11px] font-bold uppercase tracking-widest text-white hover:bg-white hover:text-black transition-all shadow-[0_0_15px_rgba(255,255,255,0.1)]">
              {{ store.lang === 'en' ? 'Visit Site' : 'Kunjungi Web' }}
            </a>
          </div>
        </div>

        <!-- Project 2: Churn Prediction -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-4 block">MACHINE LEARNING / ANALYTICS</span>
            <h3 class="text-xl font-bold text-white mb-3">Customer Churn Prediction</h3>
            <p class="text-sm text-gray-400 mb-4 font-light leading-relaxed">
              {{ store.lang === 'en' 
                ? 'Multi-model prediction system (XGBoost vs NN) featuring auto-model selection and production drift monitoring.' 
                : 'Sistem prediksi multi-model (XGBoost vs NN) dengan seleksi model otomatis dan pemantauan drift di production.' }}
            </p>
            
            <!-- CSS Metrics Chart -->
            <div class="mb-6 space-y-3 bg-white/5 p-4 rounded-xl border border-white/5">
              <div>
                <div class="flex justify-between text-[10px] text-gray-300 mb-1 font-mono"><span>AUC SCORE</span><span>0.84</span></div>
                <div class="w-full bg-black/50 rounded-full h-1.5"><div class="bg-gradient-to-r from-blue-500 to-cyan-400 h-1.5 rounded-full" style="width: 84%"></div></div>
              </div>
              <div>
                <div class="flex justify-between text-[10px] text-gray-300 mb-1 font-mono"><span>F1 SCORE</span><span>0.63</span></div>
                <div class="w-full bg-black/50 rounded-full h-1.5"><div class="bg-gradient-to-r from-purple-500 to-pink-500 h-1.5 rounded-full" style="width: 63%"></div></div>
              </div>
            </div>

            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">XGBoost</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">FastAPI</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Docker</span>
            </div>
          </div>
          <div class="mt-auto flex justify-center border-t border-white/10 pt-6">
            <a href="https://retain.ixiera.id" target="_blank" class="px-8 py-2.5 border border-white/20 rounded-full text-[11px] font-bold uppercase tracking-widest text-white hover:bg-white hover:text-black transition-all shadow-[0_0_15px_rgba(255,255,255,0.1)]">
              {{ store.lang === 'en' ? 'Visit Site' : 'Kunjungi Web' }}
            </a>
          </div>
        </div>

        <!-- Project 3: Metal Casting -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-4 block">COMPUTER VISION / QUALITY CONTROL</span>
            <h3 class="text-xl font-bold text-white mb-3">Metal Defect Inspection</h3>
            <p class="text-sm text-gray-400 mb-4 font-light leading-relaxed">
              {{ store.lang === 'en' 
                ? 'Hybrid CNN (MobileNetV2) + OpenCV system to detect and classify defect severity on metallic pump impellers.' 
                : 'Sistem Hybrid CNN (MobileNetV2) + OpenCV untuk mendeteksi tingkat keparahan cacat pada impeller pompa logam.' }}
            </p>

            <!-- CSS Metrics Chart -->
            <div class="mb-6 space-y-3 bg-white/5 p-4 rounded-xl border border-white/5">
              <div>
                <div class="flex justify-between text-[10px] text-gray-300 mb-1 font-mono"><span>ACCURACY</span><span>98.2%</span></div>
                <div class="w-full bg-black/50 rounded-full h-1.5"><div class="bg-gradient-to-r from-emerald-500 to-teal-400 h-1.5 rounded-full" style="width: 98.2%"></div></div>
              </div>
              <div class="flex gap-4">
                <div class="w-1/2">
                  <div class="flex justify-between text-[10px] text-gray-300 mb-1 font-mono"><span>PRECISION</span><span>0.98</span></div>
                  <div class="w-full bg-black/50 rounded-full h-1.5"><div class="bg-blue-500 h-1.5 rounded-full" style="width: 98%"></div></div>
                </div>
                <div class="w-1/2">
                  <div class="flex justify-between text-[10px] text-gray-300 mb-1 font-mono"><span>RECALL</span><span>0.98</span></div>
                  <div class="w-full bg-black/50 rounded-full h-1.5"><div class="bg-purple-500 h-1.5 rounded-full" style="width: 98%"></div></div>
                </div>
              </div>
            </div>

            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">TensorFlow</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">OpenCV</span>
            </div>
          </div>
          <div class="mt-auto flex justify-center border-t border-white/10 pt-6">
            <a href="https://docs.google.com/document/d/1CVAd3oWIpLsBNhHrEqfiTBe0d3T9XB5-/edit?usp=drivesdk&ouid=110367082878703692421&rtpof=true&sd=true" target="_blank" class="px-8 py-2.5 border border-white/20 rounded-full text-[11px] font-bold uppercase tracking-widest text-white hover:bg-white hover:text-black transition-all">
              {{ store.lang === 'en' ? 'View Tech Doc' : 'Lihat Dokumen' }}
            </a>
          </div>
        </div>

        <!-- Project 4: Zora AI -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase mb-4 block">AGENTIC AUTOMATION</span>
            <h3 class="text-xl font-bold text-white mb-3">Zora AI — WhatsApp Sales Agent</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              {{ store.lang === 'en' 
                ? 'Multi-agent AI system on WhatsApp for property sales automation. Architected for context-aware responses grounded in property data.' 
                : 'Sistem agen AI multi-tasking di WhatsApp untuk otomatisasi penjualan properti, terintegrasi langsung dengan basis data perusahaan.' }}
            </p>
            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">N8N</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Gemini</span>
              <span class="px-2 py-1 rounded bg-white/5 border border-white/10 text-[10px] text-gray-400">Supabase</span>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>
