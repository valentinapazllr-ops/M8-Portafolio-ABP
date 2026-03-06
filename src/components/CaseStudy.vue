<template>
  <section id="estudio" class="section case-section">
    <div class="premium-container">
      <div class="glass-card case-outer animate-reveal">
        <div class="case-columns">
          <div class="case-main">
            <span class="case-label">Caso de Estudio #01</span>
            <h2 class="case-title">{{ caseStudy.title }}</h2>
            <div class="case-intro">
              <div class="intro-block">
                <h4>Desafío</h4>
                <p>{{ caseStudy.challenge }}</p>
              </div>
              <div class="intro-block">
                <h4>Solución</h4>
                <p>{{ caseStudy.solution }}</p>
              </div>
            </div>
            <div class="case-quote">
              <p>{{ caseStudy.justification }}</p>
            </div>
          </div>
          <div class="case-sidebar">
            <div
              v-for="detail in caseStudy.details"
              :key="detail.title"
              class="sidebar-item"
            >
              <h5>{{ detail.title }}</h5>
              <ul>
                <li v-for="item in detail.items" :key="item">{{ item }}</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const props = defineProps({
  caseStudy: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
/* scoped styling may be added here later */
</style>
