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
              <div class="project-actions">
                <a
                  v-if="p.liveUrl"
                  :href="p.liveUrl"
                  target="_blank"
                  rel="noopener"
                  class="btn-action btn-live"
                >
                  <i class="fas fa-external-link-alt"></i> Demo
                </a>
                <a
                  v-if="p.repoUrl"
                  :href="p.repoUrl"
                  target="_blank"
                  rel="noopener"
                  class="btn-action btn-repo"
                >
                  <i class="fab fa-github"></i> Código
                </a>
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
.project-actions {
  display: flex;
  gap: 12px;
  margin-top: 1.5rem;
}

.btn-action {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 16px;
  border-radius: 8px;
  font-size: 0.85rem;
  font-weight: 600;
  text-decoration: none;
  transition: all 0.3s ease;
}

.btn-live {
  background: var(--gradient-primary);
  color: #fff;
}

.btn-repo {
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  color: var(--text-muted);
}

.btn-action:hover {
  transform: translateY(-3px);
  filter: brightness(1.1);
}

.btn-repo:hover {
  background: rgba(255, 255, 255, 0.1);
  color: #fff;
  border-color: rgba(255, 255, 255, 0.2);
}
</style>
