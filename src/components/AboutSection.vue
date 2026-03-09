<template>
  <section id="sobre-mi" class="section about-section">
    <div class="premium-container">
      <div class="glass-card about-card animate-reveal">
        <div class="about-grid">
          <div class="about-text-content">
            <h2 class="title-xl">
              🙋‍♀️ <span class="gradient-text">Sobre mí</span>
            </h2>
            <p class="about-lead">
              Soy desarrolladora Full Stack Junior con fuerte enfoque en el
              ecosistema Frontend moderno con Vue.js y pasión por crear
              interfaces intuitivas y de alto impacto visual.
            </p>
            <ul class="about-points">
              <li>
                <i class="fas fa-rocket"></i> Experiencia en desarrollo de SPAs
                dinámicas con Vue 3 (Composition API)
              </li>
              <li>
                <i class="fas fa-fire"></i> Gestión de datos en tiempo real con
                Firebase / Firestore
              </li>
              <li>
                <i class="fas fa-target-short"></i> Comprometida con la calidad
                del código y la experiencia del usuario (UX)
              </li>
              <li>
                <i class="fas fa-book"></i> Certificada en Desarrollo de
                Aplicaciones Front-end Trainee · ISEG / SENCE 2026
              </li>
            </ul>
          </div>

          <div class="tech-grid">
            <div class="tech-category">
              <h3>Frontend</h3>
              <div class="tech-items">
                <span>Vue.js</span>
                <span>JavaScript</span>
                <span>HTML5</span>
                <span>CSS3</span>
                <span>Responsive Design</span>
              </div>
            </div>
            <div class="tech-category">
              <h3>Herramientas</h3>
              <div class="tech-items">
                <span>Firebase</span>
                <span>Git</span>
                <span>GitHub</span>
                <span>VSCode</span>
                <span>Java</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-section {
  padding: 5rem 0;
}

.about-card {
  padding: 4rem;
}

.about-grid {
  display: grid;
  grid-template-columns: 1.2fr 0.8fr;
  gap: 4rem;
}

.about-lead {
  font-size: 1.2rem;
  margin: 2rem 0;
  color: var(--text-primary);
  line-height: 1.8;
}

.about-points {
  list-style: none;
  padding: 0;
  display: grid;
  gap: 1.2rem;
}

.about-points li {
  display: flex;
  align-items: center;
  gap: 1rem;
  color: var(--text-secondary);
  font-size: 1.05rem;
}

.about-points i {
  color: var(--accent-primary);
  width: 20px;
}

.tech-grid {
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
}

.tech-category h3 {
  font-size: 1.1rem;
  color: var(--accent-primary);
  margin-bottom: 1.2rem;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.tech-items {
  display: flex;
  flex-wrap: wrap;
  gap: 0.8rem;
}

.tech-items span {
  padding: 0.5rem 1rem;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid var(--glass-border);
  border-radius: 8px;
  font-size: 0.9rem;
  color: var(--text-secondary);
  transition: all 0.3s ease;
}

.tech-items span:hover {
  background: rgba(16, 185, 129, 0.1);
  border-color: var(--accent-primary);
  color: var(--text-primary);
}

@media (max-width: 1024px) {
  .about-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
}

@media (max-width: 768px) {
  .about-card {
    padding: 2.5rem;
  }
}
</style>
