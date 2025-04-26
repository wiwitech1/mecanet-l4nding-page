<template>
  <div class="landing-view">
    <NavbarComponent />
    <section id="home">
      <HeroComponent />
    </section>
    <section id="producto">
      <ProductComponent />
    </section>
    <section id="beneficios">
      <BenefitsComponent />
    </section>
    <section id="planes">
      <PlansComponent />
    </section>
    <section id="faq">
      <FAQComponent />
    </section>
    <FooterComponent />
  </div>
</template>

<script setup lang="ts">
import NavbarComponent from '@/components/common/NavbarComponent.vue'
import HeroComponent from '@/components/landing/HeroComponent.vue'
import ProductComponent from '@/components/landing/ProductComponent.vue'
import BenefitsComponent from '@/components/landing/BenefitsComponent.vue'
import PlansComponent from '@/components/landing/PlansComponent.vue'
import FAQComponent from '@/components/landing/FAQComponent.vue'
import FooterComponent from '@/components/common/FooterComponent.vue'
</script>

<style scoped>
.landing-view {
  background: var(--color-background);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: start;
  min-height: 100vh;
  width: 100%;
  padding: 0 8%;
  scroll-behavior: smooth;
}

section {
  width: 100%;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  scroll-margin-top: 100px; /* Ajusta esto según la altura de tu navbar */
  padding: 4rem 0;
}

/* Mejora la estética en dispositivos pequeños */
@media (max-width: 768px) {
  section {
    min-height: 80vh;
    scroll-margin-top: 80px;
    padding: 2rem 0;
  }
}
</style>
