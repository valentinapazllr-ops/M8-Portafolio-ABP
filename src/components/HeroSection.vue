<template>
  <header class="hero-section animate-reveal">
    <div class="premium-container hero-grid">
      <div class="hero-content">
        <div class="badge-new">Portfolio 2026</div>
        <h1 class="hero-main-title">
          ¡Hola! Soy <br /><span class="gradient-text">Valentina Paz 👋</span>
        </h1>
        <p class="hero-lead">
          Junior Full Stack Developer · Especialista en Vue.js & Soluciones
          Digitales
        </p>
        <p class="hero-story">
          Convierto ideas complejas en interfaces dinámicas de alto rendimiento.
        </p>

        <div class="hero-contact-info">
          <span class="contact-item"
            ><i class="fas fa-map-marker-alt"></i> Santiago, Chile</span
          >
          <span class="contact-item"
            ><i class="fas fa-briefcase"></i> Disponible para Trabajo
            Remoto</span
          >
          <span class="contact-item"
            ><i class="fas fa-envelope"></i> valentinapazll.r@gmail.com</span
          >
        </div>

        <div class="tech-stack">
          <span class="tech-tag tag-vue"
            ><i class="fab fa-vuejs"></i> Vue.js</span
          >
          <span class="tech-tag tag-js"
            ><i class="fab fa-js"></i> JavaScript</span
          >
          <span class="tech-tag tag-html"
            ><i class="fab fa-html5"></i> HTML5</span
          >
          <span class="tech-tag tag-css"
            ><i class="fab fa-css3-alt"></i> CSS3</span
          >
          <span class="tech-tag tag-firebase"
            ><i class="fas fa-fire"></i> Firebase</span
          >
          <span class="tech-tag tag-git"
            ><i class="fab fa-git-alt"></i> Git</span
          >
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
// Hero content is currently static; props can be added later if needed
</script>

<style scoped>
.hero-contact-info {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  margin-bottom: 2rem;
  color: var(--text-secondary);
  font-size: 0.95rem;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.contact-item i {
  color: var(--accent-primary);
}

.tech-stack {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 2rem;
}

.tech-tag {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 16px;
  border-radius: 12px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  font-size: 0.9rem;
  font-weight: 500;
  color: var(--text-muted);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  cursor: pointer;
  text-decoration: none;
}

.tech-tag i {
  font-size: 1.1rem;
}

.tech-tag:hover {
  transform: translateY(-5px);
  border-color: rgba(255, 255, 255, 0.3);
  color: #fff;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

/* Color accents per tag */
.tag-vue:hover {
  color: #42b883;
  border-color: #42b883;
  box-shadow: 0 5px 15px rgba(66, 184, 131, 0.2);
}
.tag-js:hover {
  color: #f7df1e;
  border-color: #f7df1e;
  box-shadow: 0 5px 15px rgba(247, 223, 30, 0.2);
}
.tag-html:hover {
  color: #e34f26;
  border-color: #e34f26;
  box-shadow: 0 5px 15px rgba(227, 79, 38, 0.2);
}
.tag-css:hover {
  color: #1572b6;
  border-color: #1572b6;
  box-shadow: 0 5px 15px rgba(21, 114, 182, 0.2);
}
.tag-sass:hover {
  color: #cc6699;
  border-color: #cc6699;
  box-shadow: 0 5px 15px rgba(204, 102, 153, 0.2);
}
.tag-firebase:hover {
  color: #ffca28;
  border-color: #ffca28;
  box-shadow: 0 5px 15px rgba(255, 202, 40, 0.2);
}
.tag-vscode:hover {
  color: #007acc;
  border-color: #007acc;
  box-shadow: 0 5px 15px rgba(0, 122, 204, 0.2);
}
</style>
