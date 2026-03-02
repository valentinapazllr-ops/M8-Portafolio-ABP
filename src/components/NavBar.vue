<template>
  <nav class="main-nav animate-reveal">
    <div class="premium-container nav-inner">
      <div class="brand">
        <span class="logo gradient-text">Valentina.</span>
      </div>
      <div class="nav-links">
        <a href="#proyectos">Work</a>
        <a href="#estudio">Case Study</a>
        <a href="#foda">Analysis</a>
        <a href="#cv">CV</a>
        <div class="nav-divider"></div>
        <div class="social-box">
          <a
            :href="contact.linkedin"
            target="_blank"
            rel="noopener"
            ><i class="fab fa-linkedin-in"></i
          ></a>
          <a :href="contact.github" target="_blank" rel="noopener"
            ><i class="fab fa-github"></i
          ></a>
          <a :href="`mailto:${contact.email}`" class="btn-email"
            >Contact</a
          >
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
