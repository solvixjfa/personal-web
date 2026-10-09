<script setup>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import AboutSkills from './components/AboutSkills.vue'
import Experience from './components/Experience.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="min-h-screen bg-[#050505] text-gray-200 font-sans selection:bg-white selection:text-black">
    <Navbar />
    <Hero />
    <AboutSkills />
    <Experience />
    <Contact />
    <Footer />
  </div>
</template>
