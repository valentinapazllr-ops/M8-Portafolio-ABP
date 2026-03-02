<template>
  <section id="archivos" class="section docs-section">
    <div class="premium-container">
      <div class="section-header">
        <h2 class="title-xl">
          Archivos <span class="gradient-text">Generados</span>
        </h2>
        <p class="section-subtitle">
          Documentación estratégica y entregables del módulo de empleabilidad.
        </p>
      </div>
      <div class="docs-grid">
        <a
          v-for="doc in docs"
          :key="doc.name"
          :href="doc.url"
          target="_blank"
          class="glass-card doc-card animate-reveal"
        >
          <div class="doc-icon">
            <i :class="doc.icon"></i>
          </div>
          <div class="doc-info">
            <span class="doc-name">{{ doc.name }}</span>
            <span class="doc-action"
              >Abrir archivo <i class="fas fa-external-link-alt"></i
            ></span>
          </div>
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
const props = defineProps({
  docs: {
    type: Array,
    required: true,
  },
});
</script>

<style scoped>
/* no extra styles yet */
</style>