<template>
  <section id="stats" class="section stats-section">
    <div class="premium-container">
      <div class="section-header">
        <h2 class="title-xl">
          📊 <span class="gradient-text">GitHub Stats</span>
        </h2>
        <p class="section-subtitle">
          Métricas de actividad y lenguajes más utilizados.
        </p>
      </div>

      <div class="stats-grid animate-reveal">
        <div class="glass-card stat-card">
          <h3>Valentina's GitHub Stats</h3>
          <div class="stat-img-container">
            <img :src="statsUrl" alt="GitHub Stats" @error="handleImgError" />
          </div>
        </div>

        <div class="glass-card stat-card">
          <h3>Top Languages</h3>
          <div class="stat-img-container">
            <img
              :src="languagesUrl"
              alt="Top Languages"
              @error="handleImgError"
            />
          </div>
        </div>
      </div>

      <div class="connect-box glass-card animate-reveal">
        <h2>🤝 <span class="gradient-text">Conectemos</span></h2>
        <div class="social-links">
          <a
            href="https://www.linkedin.com/in/valentina-paz-llantén-robles-a2684a276/"
            target="_blank"
            class="social-link linkedin"
          >
            <i class="fab fa-linkedin"></i> LinkedIn
          </a>
          <a
            href="https://github.com/valentinapazllr-ops"
            target="_blank"
            class="social-link github"
          >
            <i class="fab fa-github"></i> GitHub
          </a>
          <a href="mailto:valentinapazll.r@gmail.com" class="social-link email">
            <i class="fas fa-envelope"></i> Email
          </a>
        </div>
        <p class="footer-note">
          © 2026 · Developed with passion for the digital future 💚
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
const username = "valentinapazllr-ops";
const statsUrl = `https://github-readme-stats.vercel.app/api?username=${username}&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0f16`;
const languagesUrl = `https://github-readme-stats.vercel.app/api/top-langs/?username=${username}&layout=compact&theme=tokyonight&hide_border=true&bg_color=0a0f16`;

const handleImgError = (e) => {
  e.target.style.display = "none";
};
</script>

<style scoped>
.stats-section {
  padding: 5rem 0;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
  gap: 2rem;
  margin-bottom: 4rem;
}

.stat-card {
  padding: 2rem;
  text-align: center;
}

.stat-card h3 {
  margin-bottom: 1.5rem;
  font-size: 1.2rem;
  color: var(--text-secondary);
}

.stat-img-container img {
  width: 100%;
  max-width: 100%;
  border-radius: 12px;
}

.connect-box {
  text-align: center;
  padding: 4rem;
  margin-top: 4rem;
}

.social-links {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 2rem;
  margin: 3rem 0;
}

.social-link {
  display: flex;
  align-items: center;
  gap: 0.8rem;
  padding: 1rem 2rem;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid var(--glass-border);
  border-radius: 99px;
  text-decoration: none;
  font-weight: 600;
  color: var(--text-primary);
  transition: all 0.3s ease;
}

.social-link:hover {
  transform: translateY(-5px);
  background: rgba(16, 185, 129, 0.1);
  border-color: var(--accent-primary);
}

.social-link i {
  font-size: 1.4rem;
}

.linkedin:hover i {
  color: #0077b5;
}
.github:hover i {
  color: #fff;
}
.email:hover i {
  color: #ea4335;
}

.footer-note {
  margin-top: 3rem;
  color: var(--text-secondary);
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .stats-grid {
    grid-template-columns: 1fr;
  }
}
</style>
