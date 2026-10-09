<script setup>
import { store } from '../store.js'
</script>

<template>
  <section id="experience" class="py-20 border-t border-white/5 bg-[#080808]">
    <div class="max-w-4xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-[10px] font-mono tracking-[0.3em] text-gray-500 uppercase mb-3">
          {{ store.lang === 'en' ? 'Background' : 'Rekam Jejak' }}
        </h2>
        <p class="text-2xl sm:text-3xl font-bold text-white">
          {{ store.lang === 'en' ? 'Where I\'ve Been' : 'Pengalaman Kerja' }}
        </p>
      </div>

      <div class="space-y-8">
        <!-- Job 1 -->
        <div class="p-8 rounded-2xl border border-white/10 bg-[#0a0a0a]">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-4">
            <h3 class="text-lg font-bold text-white">AI Engineer & Fullstack Developer</h3>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase">IXIERA.ID | JAN 2025 - PRESENT</span>
          </div>
          <div v-if="store.lang === 'en'" class="space-y-3 text-sm text-gray-400 font-light leading-relaxed">
            <p>&mdash; Built an AI Sales Agent from scratch using LangGraph and a RAG pipeline.</p>
            <p>&mdash; Developed a client portal to track projects in real-time (Next.js + Supabase).</p>
            <p>&mdash; Set up backend endpoints with FastAPI and ran LLM fine-tuning experiments right on production data.</p>
          </div>
          <div v-else class="space-y-3 text-sm text-gray-400 font-light leading-relaxed">
            <p>&mdash; Ngebangun AI Sales Agent dari nol pakai arsitektur LangGraph dan RAG.</p>
            <p>&mdash; Develop portal klien (Next.js + Supabase) biar mereka gampang mantau progres proyek.</p>
            <p>&mdash; Bikin backend AI pakai FastAPI dan ngelakuin eksperimen fine-tuning LLM pakai data asli dari lapangan.</p>
          </div>
        </div>

        <!-- Job 2 -->
        <div class="p-8 rounded-2xl border border-white/5 bg-transparent">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-4">
            <h3 class="text-lg font-bold text-white">AI Automation Engineer</h3>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase">PT KARYA GRAHA PRIMANUSA | JAN - APR 2026</span>
          </div>
          <div v-if="store.lang === 'en'" class="space-y-3 text-sm text-gray-400 font-light leading-relaxed">
            <p>&mdash; Rolled out Zora AI on WhatsApp to handle property sales across 5 different projects.</p>
            <p>&mdash; Hooked up N8N, Chatwoot, and Supabase on a self-hosted Coolify VPS to keep things fast and secure.</p>
          </div>
          <div v-else class="space-y-3 text-sm text-gray-400 font-light leading-relaxed">
            <p>&mdash; Terapin sistem Zora AI di WhatsApp buat ngotomatisasi jualan di 5 proyek properti sekaligus.</p>
            <p>&mdash; Ngerancang infrastrukturnya di atas VPS sendiri pakai N8N dan Chatwoot biar lebih aman dan hemat *cost*.</p>
          </div>
        </div>

        <!-- Job 3 -->
        <div class="p-8 rounded-2xl border border-white/5 bg-transparent opacity-75">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-4">
            <h3 class="text-lg font-bold text-white">Cleaning Service Staff</h3>
            <span class="text-[10px] font-mono tracking-widest text-gray-500 uppercase">PENDAWA | 2023 - 2024</span>
          </div>
          <div v-if="store.lang === 'en'" class="space-y-3 text-sm text-gray-400 font-light leading-relaxed">
            <p>&mdash; Where I learned the value of strict SOPs, hard work, and maintaining high operational standards before jumping into tech.</p>
          </div>
          <div v-else class="space-y-3 text-sm text-gray-400 font-light leading-relaxed">
            <p>&mdash; Tempat saya belajar soal disiplin, kerja keras, dan pentingnya ngikutin SOP (Standar Operasional) yang ketat sebelum masuk ke dunia *tech*.</p>
          </div>
        </div>
      </div>

      <!-- Edu -->
      <div class="mt-20">
        <h3 class="text-[10px] font-mono tracking-[0.3em] text-gray-500 uppercase mb-8 text-center">
          {{ store.lang === 'en' ? 'Education & Certifications' : 'Pendidikan & Sertifikasi' }}
        </h3>
        <div class="grid sm:grid-cols-3 gap-6">
          <div class="border border-white/10 p-6 rounded-xl bg-white/[0.01] text-center">
            <h4 class="text-sm font-bold text-white mb-2">Machine Learning Specialization</h4>
            <p class="text-[10px] font-mono text-gray-500">DeepLearning.AI | 2026</p>
          </div>
          <div class="border border-white/10 p-6 rounded-xl bg-white/[0.01] text-center">
            <h4 class="text-sm font-bold text-white mb-2">Machine Learning Credentials</h4>
            <p class="text-[10px] font-mono text-gray-500">IBM SkillsBuild | 2026</p>
          </div>
          <div class="border border-white/10 p-6 rounded-xl bg-white/[0.01] text-center">
            <h4 class="text-sm font-bold text-white mb-2">Computer Engineering</h4>
            <p class="text-[10px] font-mono text-gray-500">SMKN 1 Prigen | 2022</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
