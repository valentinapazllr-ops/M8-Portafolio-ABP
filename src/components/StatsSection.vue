<template>
  <section id="contacto" class="section contact-section">
    <div class="premium-container">
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

<script setup></script>

<style scoped>
.contact-section {
  padding: 5rem 0;
}

.connect-box {
  text-align: center;
  padding: 4rem;
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
</style>
