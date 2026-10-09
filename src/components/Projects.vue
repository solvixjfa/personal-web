<template>
  <section id="projects" class="py-20 border-t border-white/5 bg-[#080808]">
    <div class="max-w-5xl mx-auto px-6">
      <div class="text-center mb-16">
        <h2 class="text-xs font-bold tracking-[0.3em] text-gray-400 uppercase mb-3">FEATURED WORK</h2>
        <p class="text-2xl sm:text-3xl font-bold text-white">Selected Projects & Systems</p>
      </div>

      <div class="grid md:grid-cols-2 gap-8">
        
        <!-- Project 1: Niki CoC Bot (SaaS) -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between mb-4">
              <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">COMMUNITY SAAS / DISCORD BOT</span>
              <a href="https://coc.ixiera.id" target="_blank" class="text-xs font-bold text-white hover:underline flex items-center gap-1">
                VISIT SITE &rarr;
              </a>
            </div>
            <h3 class="text-xl font-bold text-white mb-3">Niki CoC Bot</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Autonomous Discord bot for Clash of Clans management. Features real-time war updates, CWL analytics, donation tracking, and AI-powered clan health audits.
            </p>
            <div class="text-xs font-mono text-gray-400 mb-6 space-y-1">
              <div>Python &bull; Discord API &bull; Gemini API &bull; Vue 3 &bull; Vite &bull; Vercel</div>
            </div>
          </div>
        </div>

        <!-- Project 2: Customer Churn Prediction (Live) -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between mb-4">
              <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">MACHINE LEARNING / ANALYTICS</span>
              <a href="https://retain.ixiera.id" target="_blank" class="text-xs font-bold text-white hover:underline flex items-center gap-1">
                VISIT SITE &rarr;
              </a>
            </div>
            <h3 class="text-xl font-bold text-white mb-3">Customer Churn Prediction System</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Multi-model churn prediction system (XGBoost vs Neural Network) featuring auto-model selection, K-Means customer segmentation, LLM explanations, and production drift monitoring.
            </p>
            <div class="text-xs font-mono text-gray-400 mb-4 space-y-1">
              <div>Metrics: F1 0.63 | AUC 0.84</div>
              <div>XGBoost &bull; TensorFlow &bull; MLflow &bull; FastAPI &bull; Docker &bull; Railway</div>
            </div>
          </div>
        </div>

        <!-- Project 3: Metal Casting Defect Inspection -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between mb-4">
              <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">COMPUTER VISION / QUALITY CONTROL</span>
            </div>
            <h3 class="text-xl font-bold text-white mb-3">Automated Metal Defect Inspection</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Hybrid CNN (MobileNetV2) + OpenCV + Random Forest system to detect and classify defect severity on metallic pump impellers in real-time.
            </p>
            <div class="text-xs font-mono text-gray-400 mb-4 space-y-1">
              <div>Metrics: Accuracy 98.2% | Precision 0.98 | Recall 0.98</div>
              <div>TensorFlow &bull; OpenCV &bull; scikit-learn &bull; Gradio &bull; Python</div>
            </div>
          </div>
        </div>

        <!-- Project 4: Zora AI (Enterprise / WhatsApp Automation) -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between mb-4">
              <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">ENTERPRISE / AGENTIC AUTOMATION</span>
            </div>
            <h3 class="text-xl font-bold text-white mb-3">Zora AI — WhatsApp Sales Agent</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Agentic AI system on WhatsApp for property sales automation across 5 active real-estate projects. Multi-agent orchestration grounded in property data.
            </p>
            <div class="text-xs font-mono text-gray-400 mb-4 space-y-1">
              <div>Impact: Automating sales for Woodland Group</div>
              <div>N8N &bull; Chatwoot &bull; Evolution API &bull; Groq &bull; Gemini &bull; Supabase</div>
            </div>
          </div>
        </div>

        <!-- Project 5: Personal Finance Anomaly Detection -->
        <div class="glossy-card p-8 rounded-2xl flex flex-col justify-between md:col-span-2">
          <div>
            <div class="flex items-center justify-between mb-4">
              <span class="text-[10px] font-mono tracking-widest text-gray-400 uppercase">AI BACKEND / ANOMALY DETECTION</span>
            </div>
            <h3 class="text-xl font-bold text-white mb-3">Personal Finance Anomaly Detection System</h3>
            <p class="text-sm text-gray-400 mb-6 font-light leading-relaxed">
              Suspicious transaction detection system from PDF/CSV/Excel financial statements using hybrid Isolation Forest + personal baseline filtering, accompanied by Gemini API LLM explanations.
            </p>
            <div class="text-xs font-mono text-gray-400 space-y-1">
              <div>Metrics: Precision 0.81 | Recall 0.78 | F1 0.79</div>
              <div>scikit-learn &bull; FastAPI &bull; pdfplumber &bull; Gemini API &bull; Docker &bull; Railway</div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>
