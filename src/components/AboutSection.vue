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
                <span class="tech-pill tag-vue"
                  ><i class="fab fa-vuejs"></i> Vue.js</span
                >
                <span class="tech-pill tag-js"
                  ><i class="fab fa-js"></i> JavaScript</span
                >
                <span class="tech-pill tag-html"
                  ><i class="fab fa-html5"></i> HTML5</span
                >
                <span class="tech-pill tag-css"
                  ><i class="fab fa-css3-alt"></i> CSS3</span
                >
                <span class="tech-pill tag-responsive"
                  ><i class="fas fa-mobile-alt"></i> Responsive Design</span
                >
              </div>
            </div>
            <div class="tech-category">
              <h3>Herramientas</h3>
              <div class="tech-items">
                <span class="tech-pill tag-firebase"
                  ><i class="fas fa-fire"></i> Firebase</span
                >
                <span class="tech-pill tag-git"
                  ><i class="fab fa-git-alt"></i> Git</span
                >
                <span class="tech-pill tag-github"
                  ><i class="fab fa-github"></i> GitHub</span
                >
                <span class="tech-pill tag-vscode"
                  ><i class="fas fa-code"></i> VSCode</span
                >
                <span class="tech-pill tag-java"
                  ><i class="fab fa-java"></i> Java</span
                >
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
  gap: 1rem;
}

.tech-pill {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 16px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid var(--glass-border);
  border-radius: 12px;
  font-size: 0.9rem;
  font-weight: 500;
  color: var(--text-secondary);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  cursor: default;
}

.tech-pill i {
  font-size: 1.1rem;
}

.tech-pill:hover {
  transform: translateY(-3px);
  background: rgba(255, 255, 255, 0.1);
  color: #fff;
}

/* Personalized Colors per Tag */
.tag-vue:hover {
  color: #42b883;
  border-color: #42b883;
  background: rgba(66, 184, 131, 0.1);
}
.tag-js:hover {
  color: #f7df1e;
  border-color: #f7df1e;
  background: rgba(247, 223, 30, 0.1);
}
.tag-html:hover {
  color: #e34f26;
  border-color: #e34f26;
  background: rgba(227, 79, 38, 0.1);
}
.tag-css:hover {
  color: #1572b6;
  border-color: #1572b6;
  background: rgba(21, 114, 182, 0.1);
}
.tag-responsive:hover {
  color: #10b981;
  border-color: #10b981;
  background: rgba(16, 185, 129, 0.1);
}
.tag-firebase:hover {
  color: #ffca28;
  border-color: #ffca28;
  background: rgba(255, 202, 40, 0.1);
}
.tag-git:hover {
  color: #f05032;
  border-color: #f05032;
  background: rgba(240, 80, 50, 0.1);
}
.tag-github:hover {
  color: #fff;
  border-color: rgba(255, 255, 255, 0.5);
  background: rgba(255, 255, 255, 0.1);
}
.tag-vscode:hover {
  color: #007acc;
  border-color: #007acc;
  background: rgba(0, 122, 204, 0.1);
}
.tag-java:hover {
  color: #007396;
  border-color: #007396;
  background: rgba(0, 115, 150, 0.1);
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
