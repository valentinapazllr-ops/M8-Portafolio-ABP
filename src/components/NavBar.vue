<template>
  <nav class="main-nav animate-reveal">
    <div class="premium-container nav-inner">
      <div class="brand">
        <span class="logo gradient-text">Valentina.</span>
      </div>
      <div class="nav-links">
        <a href="#proyectos">Proyectos</a>
        <a href="#sobre-mi">Sobre mí</a>
        <a href="#contacto">Contacto</a>
        <div class="nav-divider"></div>
        <div class="social-box">
          <a :href="contact.linkedin" target="_blank" rel="noopener"
            ><i class="fab fa-linkedin-in"></i
          ></a>
          <a :href="contact.github" target="_blank" rel="noopener"
            ><i class="fab fa-github"></i
          ></a>
          <a :href="`mailto:${contact.email}`" class="btn-email">Contacto</a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup>
// `contact` object contains linkedin, github and email strings
const props = defineProps({
  contact: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
/* scoped rules can be added here if nav requires overrides */
</style>
