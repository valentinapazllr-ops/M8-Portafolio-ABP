<template>
  <section id="proyectos" class="section work-section">
    <div class="premium-container">
      <div class="section-header">
        <h2 class="title-xl">
          Proyectos <span class="gradient-text">Destacados</span>
        </h2>
        <p class="section-subtitle">
          Selección de proyectos destacados en desarrollo de software.
        </p>
      </div>
      <div class="projects-grid">
        <div
          v-for="p in projects"
          :key="p.id"
          class="project-wrapper animate-reveal"
        >
          <div class="glass-card project-card">
            <div class="img-container">
              <img
                :src="p.image"
                :alt="p.title"
                class="project-img"
                @error="(e) => (e.target.src = 'https://picsum.photos/600/400')"
              />
            </div>
            <div class="project-info">
              <h3 class="p-title">{{ p.title }}</h3>
              <p class="p-desc">{{ p.description }}</p>
              <div class="p-tags">
                <span v-for="tag in p.tags" :key="tag" class="tag-pill">
                  {{ tag }}</span
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const props = defineProps({
  projects: {
    type: Array,
    required: true,
  },
});
</script>

<style scoped>
/* add component specific styles if desired */
</style>
