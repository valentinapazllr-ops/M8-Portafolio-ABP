<template>
  <section id="foda" class="section foda-section">
    <div class="premium-container">
      <div class="section-header">
        <h2 class="title-xl">
          Análisis <span class="gradient-text">Estratégico</span>
        </h2>
        <p class="section-subtitle">
          Matriz FODA aplicada al perfil profesional IT.
        </p>
      </div>
      <div class="foda-quadrants">
        <div class="foda-q glass-card green-q animate-reveal">
          <div class="q-header"><i class="fas fa-arrow-up"></i> Fortalezas</div>
          <ul>
            <li v-for="item in foda.fortalezas" :key="item">{{ item }}</li>
          </ul>
        </div>
        <div class="foda-q glass-card blue-q animate-reveal">
          <div class="q-header"><i class="fas fa-star"></i> Oportunidades</div>
          <ul>
            <li v-for="item in foda.oportunidades" :key="item">{{ item }}</li>
          </ul>
        </div>
        <div class="foda-q glass-card red-q animate-reveal">
          <div class="q-header">
            <i class="fas fa-exclamation-triangle"></i> Debilidades
          </div>
          <ul>
            <li v-for="item in foda.debilidades" :key="item">{{ item }}</li>
          </ul>
        </div>
        <div class="foda-q glass-card orange-q animate-reveal">
          <div class="q-header"><i class="fas fa-shield-alt"></i> Amenazas</div>
          <ul>
            <li v-for="item in foda.amenazas" :key="item">{{ item }}</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const props = defineProps({
  foda: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
/* optional scoped rules */
</style>
