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
        <h2 class="text-[10px] font-mono tracking-[0.3em] text-gray-500 uppercase mb-3">
          {{ store.lang === 'en' ? 'The Approach' : 'Cara Kerja' }}
        </h2>
        <p class="text-2xl sm:text-3xl font-bold text-white max-w-3xl mx-auto leading-tight">
          {{ store.lang === 'en' 
            ? 'Bridging the gap between raw engineering and business logic.'
            : 'Menjembatani kode teknis dengan kebutuhan bisnis yang nyata.' }}
        </p>
      </div>

      <div class="glossy-card p-8 rounded-2xl mb-16 text-center max-w-3xl mx-auto border border-white/10">
        <p v-if="store.lang === 'en'" class="text-gray-300 text-base leading-relaxed font-light">
          I don't just write code for the sake of it. I focus on building solid pipelines and ecosystems. Whether it's setting up a LangGraph flow, an optimized LLM, or a FastAPI backend, the goal is always the same: making sure it runs perfectly in production.
        </p>
        <p v-else class="text-gray-300 text-base leading-relaxed font-light">
          Bagi saya, ini bukan sekadar nulis barisan kode. Saya fokus ngebangun ekosistem yang solid. Entah itu ngeracik alur LangGraph, ngoprek LLM, atau nyiapin backend pakai FastAPI, tujuannya cuma satu: mastiin sistemnya jalan mulus pas dipakai *user*.
        </p>
      </div>

      <!-- Skills Badges (Strict Minimalist B&W) -->
      <div id="skills" class="grid md:grid-cols-2 gap-8">
        <div class="p-8 rounded-2xl border border-white/5 bg-white/[0.02]">
          <h3 class="text-xs font-mono tracking-widest text-white uppercase mb-6">AI & Machine Learning</h3>
          <div class="flex flex-wrap gap-2">
            <span v-for="s in [...skills.ai, ...skills.ml]" :key="s" class="px-3 py-1.5 rounded-full border border-white/20 text-[10px] text-gray-300 font-mono tracking-wide">
              {{ s }}
            </span>
          </div>
        </div>

        <div class="p-8 rounded-2xl border border-white/5 bg-white/[0.02]">
          <h3 class="text-xs font-mono tracking-widest text-white uppercase mb-6">Backend & Web</h3>
          <div class="flex flex-wrap gap-2">
            <span v-for="s in [...skills.backend, ...skills.web]" :key="s" class="px-3 py-1.5 rounded-full border border-white/20 text-[10px] text-gray-300 font-mono tracking-wide">
              {{ s }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
