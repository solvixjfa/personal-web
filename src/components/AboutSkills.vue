<script setup>
import { store } from '../store.js'

const skills = {
  ai: ['LangGraph', 'LangChain', 'N8N', 'RAG (pgvector)', 'Hugging Face', 'Groq API', 'Gemini', 'OpenAI'],
  ml: ['PyTorch', 'TensorFlow', 'scikit-learn', 'XGBoost', 'LLM Fine-tuning', 'Feature Engineering'],
  backend: ['Python', 'FastAPI', 'PostgreSQL', 'Docker', 'Supabase', 'Firebase'],
  web: ['Next.js', 'Vue 3', 'TypeScript', 'React', 'Vercel']
}
</script>

<template>
  <section id="about" class="py-20 border-t border-white/5 bg-[#080808]">
    <div class="max-w-5xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-xs font-bold tracking-[0.3em] text-gray-400 uppercase mb-3">
          {{ store.lang === 'en' ? 'System Architecture' : 'Arsitektur Sistem' }}
        </h2>
        <p class="text-2xl sm:text-3xl font-bold text-white max-w-3xl mx-auto leading-tight">
          {{ store.lang === 'en' 
            ? 'Translating complex business logic into autonomous systems.'
            : 'Menerjemahkan logika bisnis yang kompleks menjadi sistem otonom.' }}
        </p>
      </div>

      <div class="glossy-card p-8 rounded-2xl mb-16 text-center max-w-3xl mx-auto">
        <p v-if="store.lang === 'en'" class="text-gray-300 text-base leading-relaxed font-light">
          I don't just write code; I design pipelines. Bridging the gap between raw engineering requirements and real-world business needs using LangGraph, FastAPI, and optimized LLMs.
        </p>
        <p v-else class="text-gray-300 text-base leading-relaxed font-light">
          Bukan sekadar menulis kode, saya merancang ekosistem. Menjembatani kebutuhan teknis dan target bisnis nyata menggunakan LangGraph, FastAPI, dan optimalisasi LLM.
        </p>
      </div>

      <!-- Skills Badges -->
      <div id="skills" class="grid md:grid-cols-2 gap-8">
        <div class="glossy-card p-8 rounded-2xl">
          <h3 class="text-sm font-bold tracking-widest text-white uppercase mb-4">AI & Machine Learning</h3>
          <div class="flex flex-wrap gap-2 mb-8">
            <span v-for="s in [...skills.ai, ...skills.ml]" :key="s" class="px-3 py-1.5 rounded-md border border-white/10 bg-white/5 text-[11px] text-gray-300 font-mono flex items-center gap-2">
              <span class="w-1.5 h-1.5 rounded-full bg-blue-500/80"></span>{{ s }}
            </span>
          </div>
        </div>

        <div class="glossy-card p-8 rounded-2xl">
          <h3 class="text-sm font-bold tracking-widest text-white uppercase mb-4">Backend & Web Engineering</h3>
          <div class="flex flex-wrap gap-2">
            <span v-for="s in [...skills.backend, ...skills.web]" :key="s" class="px-3 py-1.5 rounded-md border border-white/10 bg-white/5 text-[11px] text-gray-300 font-mono flex items-center gap-2">
              <span class="w-1.5 h-1.5 rounded-full bg-purple-500/80"></span>{{ s }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
