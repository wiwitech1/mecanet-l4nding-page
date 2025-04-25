<template>
  <div class="landing-view">
    <NavbarComponent />
    <HeroComponent />
    <ProductComponent />


  </div>
</template>

<script setup lang="ts">
import NavbarComponent from '@/components/common/NavbarComponent.vue'
import HeroComponent from '@/components/landing/HeroComponent.vue'
import ProductComponent from '@/components/landing/ProductComponent.vue'


</script>

<style scoped>
.landing-view {
  background: var(--color-background);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: start;
  min-height: 100vh;
  width: 100vw;
  padding: 0 8%;
}
</style>
