<template>
  <section id="experience" class="py-20 border-t border-white/5 bg-[#050505]">
    <div class="max-w-4xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-xs font-bold tracking-[0.3em] text-gray-400 uppercase mb-3">BACKGROUND</h2>
        <p class="text-2xl sm:text-3xl font-bold text-white">Work Experience & Credentials</p>
      </div>

      <div class="space-y-8">
        <!-- Job 1 -->
        <div class="glossy-card p-8 rounded-2xl border-l-4 border-l-white">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-4">
            <h3 class="text-lg font-bold text-white">AI Engineer & Fullstack Developer</h3>
            <span class="text-xs font-mono tracking-widest text-gray-400">IXIERA.ID | JAN 2025 - PRESENT</span>
          </div>
          <ul class="space-y-2 text-sm text-gray-300 list-disc list-inside leading-relaxed font-light">
            <li>Designed and built an end-to-end AI Sales Agent using LangGraph, RAG pipeline with pgvector + HuggingFace, and Groq API.</li>
            <li>Developed a client portal (Next.js + Supabase + Clerk Auth) with a real-time tracking dashboard.</li>
            <li>Built a backend AI service with FastAPI + Python, deployed as a production inference endpoint.</li>
            <li>Ran LLM fine-tuning experiments (Qwen2.5, LoRA/PEFT) on production data and built an LLM-as-judge evaluation framework.</li>
          </ul>
        </div>

        <!-- Job 2 -->
        <div class="glossy-card p-8 rounded-2xl border-l-4 border-l-white/40">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-4">
            <h3 class="text-lg font-bold text-white">AI Automation Engineer</h3>
            <span class="text-xs font-mono tracking-widest text-gray-400">PT KARYA GRAHA PRIMANUSA | JAN 2026 - APR 2026</span>
          </div>
          <ul class="space-y-2 text-sm text-gray-300 list-disc list-inside leading-relaxed font-light">
            <li>Implemented an agentic AI system (Zora AI) on WhatsApp for property sales automation across 5 active projects.</li>
            <li>Designed architecture using N8N, Chatwoot, Evolution API, and Supabase on a Coolify VPS.</li>
            <li>Integrated Groq (Llama 3) and Gemini Flash 2.5 for context-aware responses grounded in property data.</li>
            <li>Authored PRD, technical architecture, and deployment guidelines.</li>
          </ul>
        </div>

        <!-- Job 3 -->
        <div class="glossy-card p-8 rounded-2xl border-l-4 border-l-white/20">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-4">
            <h3 class="text-lg font-bold text-white">Cleaning Service Staff</h3>
            <span class="text-xs font-mono tracking-widest text-gray-400">PENDAWA | 2023 - 2024</span>
          </div>
          <ul class="space-y-2 text-sm text-gray-300 list-disc list-inside leading-relaxed font-light">
            <li>Maintained high standards of cleanliness and performed routine inspections to ensure SOP compliance.</li>
          </ul>
        </div>
      </div>

      <!-- Certifications -->
      <div class="mt-16">
        <h3 class="text-xs font-bold tracking-[0.3em] text-gray-400 uppercase mb-8 text-center">EDUCATION & CERTIFICATIONS</h3>
        <div class="grid sm:grid-cols-3 gap-6">
          <div class="glossy-card p-6 rounded-xl">
            <h4 class="text-sm font-bold text-white mb-2">Machine Learning Specialization</h4>
            <p class="text-xs text-gray-400">Stanford Online / DeepLearning.AI | 2026</p>
          </div>
          <div class="glossy-card p-6 rounded-xl">
            <h4 class="text-sm font-bold text-white mb-2">Machine Learning Credentials</h4>
            <p class="text-xs text-gray-400">IBM SkillsBuild | 2026</p>
          </div>
          <div class="glossy-card p-6 rounded-xl">
            <h4 class="text-sm font-bold text-white mb-2">Computer Engineering</h4>
            <p class="text-xs text-gray-400">SMK Negeri 1 Prigen | Graduated 2022</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
