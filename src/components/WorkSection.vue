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

      <div class="view-more-container animate-reveal">
        <div class="glass-card cta-card">
          <div class="cta-content">
            <h3 class="cta-title">¿Quieres ver más?</h3>
            <p class="cta-text">
              Explora mi historial completo de proyectos y contribuciones en mi
              perfil de GitHub.
            </p>
          </div>
          <a
            href="https://github.com/valentinapazllr-ops?tab=repositories"
            target="_blank"
            rel="noopener"
            class="btn-primary btn-view-more"
          >
            <i class="fab fa-github"></i> Ver todos los repositorios
          </a>
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
.view-more-container {
  margin-top: 5rem;
}

.cta-card {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 3rem 4rem;
  background: rgba(16, 185, 129, 0.03);
  border-color: rgba(16, 185, 129, 0.2);
}

.cta-title {
  font-size: 1.8rem;
  margin-bottom: 0.5rem;
}

.cta-text {
  color: var(--text-secondary);
  font-size: 1.1rem;
}

.btn-view-more {
  display: flex;
  align-items: center;
  gap: 12px;
  white-space: nowrap;
}

.btn-view-more i {
  font-size: 1.2rem;
}

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

@media (max-width: 1024px) {
  .cta-card {
    flex-direction: column;
    text-align: center;
    gap: 2rem;
    padding: 3rem;
  }
}
</style>
