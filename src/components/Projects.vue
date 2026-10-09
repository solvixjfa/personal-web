<script setup>
import { store } from '../store.js'
</script>

<template>
  <section id="projects" class="py-20 border-t border-white/5 bg-[#050505]">
    <div class="max-w-5xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-[10px] font-mono tracking-[0.3em] text-gray-500 uppercase mb-3">
          {{ store.lang === 'en' ? 'Featured Work' : 'Karya & Proyek' }}
        </h2>
      </div>

      <div class="grid md:grid-cols-2 gap-8">
        
        <!-- Project 1: Niki CoC -->
        <div class="glossy-card p-8 rounded-2xl border border-white/10 flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-4 block">COMMUNITY SAAS</span>
            <h3 class="text-xl font-bold text-white mb-3">Niki CoC Bot</h3>
            <p v-if="store.lang === 'en'" class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              A Discord bot I built to handle the heavy lifting for Clash of Clans communities. It tracks wars, analyzes CWL data, and uses AI to audit clan health automatically so leaders don't have to.
            </p>
            <p v-else class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Bot Discord yang saya bikin khusus buat ngurusin hal-hal ribet di clan Clash of Clans. Mulai dari update skor war, rekap data CWL, sampai pakai AI buat ngecek mana member yang aktif atau sekadar numpang.
            </p>
            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">Python</span>
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">Vue 3</span>
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">Gemini AI</span>
            </div>
          </div>
          <div class="mt-auto flex justify-center border-t border-white/5 pt-6">
            <a href="https://coc.ixiera.id" target="_blank" class="px-8 py-2.5 bg-white text-black rounded text-[10px] font-bold uppercase tracking-widest hover:bg-gray-200 transition-all">
              {{ store.lang === 'en' ? 'Visit Site' : 'Kunjungi Web' }}
            </a>
          </div>
        </div>

        <!-- Project 2: Churn Prediction -->
        <div class="glossy-card p-8 rounded-2xl border border-white/10 flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-4 block">MACHINE LEARNING</span>
            <h3 class="text-xl font-bold text-white mb-3">Customer Churn Prediction</h3>
            <p v-if="store.lang === 'en'" class="text-sm text-gray-400 mb-4 font-light leading-relaxed">
              Figuring out why customers leave before they actually do. This is a multi-model system (XGBoost vs NN) that automatically selects the best algorithm and monitors data drift.
            </p>
            <p v-else class="text-sm text-gray-400 mb-4 font-light leading-relaxed">
              Sistem prediksi buat cari tahu alasan pelanggan kabur sebelum mereka beneran pergi. Pakai beberapa model sekaligus (XGBoost & NN) dan bisa milih algoritma terbaik secara otomatis.
            </p>
            
            <!-- Minimalist B&W Metrics Chart -->
            <div class="mb-6 space-y-3 bg-white/[0.02] p-4 rounded-xl border border-white/5">
              <div>
                <div class="flex justify-between text-[10px] text-gray-400 mb-1 font-mono"><span>AUC SCORE</span><span>0.84</span></div>
                <div class="w-full bg-white/10 h-1"><div class="bg-white h-1" style="width: 84%"></div></div>
              </div>
              <div>
                <div class="flex justify-between text-[10px] text-gray-400 mb-1 font-mono"><span>F1 SCORE</span><span>0.63</span></div>
                <div class="w-full bg-white/10 h-1"><div class="bg-gray-400 h-1" style="width: 63%"></div></div>
              </div>
            </div>

            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">XGBoost</span>
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">FastAPI</span>
            </div>
          </div>
          <div class="mt-auto flex justify-center border-t border-white/5 pt-6">
            <a href="https://retain.ixiera.id" target="_blank" class="px-8 py-2.5 bg-white text-black rounded text-[10px] font-bold uppercase tracking-widest hover:bg-gray-200 transition-all">
              {{ store.lang === 'en' ? 'Visit Site' : 'Kunjungi Web' }}
            </a>
          </div>
        </div>

        <!-- Project 3: Metal Casting -->
        <div class="glossy-card p-8 rounded-2xl border border-white/10 flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-4 block">COMPUTER VISION</span>
            <h3 class="text-xl font-bold text-white mb-3">Metal Defect Inspection</h3>
            <p v-if="store.lang === 'en'" class="text-sm text-gray-400 mb-4 font-light leading-relaxed">
              Trained a hybrid CNN model (MobileNetV2) to spot and classify tiny defects on metallic pump impellers, reducing the need for manual quality control checks.
            </p>
            <p v-else class="text-sm text-gray-400 mb-4 font-light leading-relaxed">
              Ngelatih model Hybrid CNN (MobileNetV2) buat nge-scan dan ngeklasifikasi cacat kecil di logam impeller pompa. Cukup ngebantu ngurangin pengecekan manual yang makan waktu.
            </p>

            <!-- Minimalist B&W Metrics -->
            <div class="mb-6 space-y-3 bg-white/[0.02] p-4 rounded-xl border border-white/5">
              <div>
                <div class="flex justify-between text-[10px] text-gray-400 mb-1 font-mono"><span>ACCURACY</span><span>98.2%</span></div>
                <div class="w-full bg-white/10 h-1"><div class="bg-white h-1" style="width: 98.2%"></div></div>
              </div>
              <div class="flex gap-4">
                <div class="w-1/2">
                  <div class="flex justify-between text-[10px] text-gray-400 mb-1 font-mono"><span>PRECISION</span><span>0.98</span></div>
                  <div class="w-full bg-white/10 h-1"><div class="bg-gray-400 h-1" style="width: 98%"></div></div>
                </div>
                <div class="w-1/2">
                  <div class="flex justify-between text-[10px] text-gray-400 mb-1 font-mono"><span>RECALL</span><span>0.98</span></div>
                  <div class="w-full bg-white/10 h-1"><div class="bg-gray-400 h-1" style="width: 98%"></div></div>
                </div>
              </div>
            </div>
          </div>
          <div class="mt-auto flex justify-center border-t border-white/5 pt-6">
            <a href="https://docs.google.com/document/d/1CVAd3oWIpLsBNhHrEqfiTBe0d3T9XB5-/edit?usp=drivesdk&ouid=110367082878703692421&rtpof=true&sd=true" target="_blank" class="px-8 py-2.5 bg-transparent border border-white text-white rounded text-[10px] font-bold uppercase tracking-widest hover:bg-white hover:text-black transition-all">
              {{ store.lang === 'en' ? 'View Tech Doc' : 'Lihat Dokumen' }}
            </a>
          </div>
        </div>

        <!-- Project 4: Zora AI -->
        <div class="glossy-card p-8 rounded-2xl border border-white/10 flex flex-col justify-between group hover:-translate-y-1 transition-transform duration-300">
          <div>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase mb-4 block">BUSINESS AUTOMATION</span>
            <h3 class="text-xl font-bold text-white mb-3">Zora AI — WhatsApp Agent</h3>
            <p v-if="store.lang === 'en'" class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Built a multi-agent system on WhatsApp to handle property sales. It chats with potential buyers, answers context-specific questions, and manages leads 24/7 without human intervention.
            </p>
            <p v-else class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Sistem AI multi-tasking di WhatsApp khusus buat otomatisasi penjualan properti. Bisa ngobrol sama calon pembeli dan ngurusin prospek 24/7 tanpa capek.
            </p>
            <div class="flex flex-wrap gap-2 mb-8">
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">N8N</span>
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">Gemini</span>
              <span class="px-2 py-1 rounded-sm border border-white/20 text-[9px] text-gray-400 font-mono">Supabase</span>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>
