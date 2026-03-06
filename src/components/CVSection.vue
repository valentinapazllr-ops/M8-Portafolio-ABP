<template>
  <section id="cv" class="section cv-section">
    <div class="premium-container">
      <div class="section-header">
        <h2 class="title-xl">
          Curriculum <span class="gradient-text">Vitae</span>
        </h2>
        <p class="section-subtitle">
          Detalle de mi trayectoria profesional y competencias técnicas.
        </p>
      </div>

      <div class="glass-card cv-container animate-reveal">
        <div class="cv-header-info">
          <h3 class="cv-name">{{ cv.name }}</h3>
          <p class="cv-tagline">{{ cv.title }}</p>
          <div class="cv-contact-row">
            <span class="cv-contact-item"
              ><i class="fas fa-map-marker-alt"></i> {{ cv.location }}</span
            >
            <span class="cv-contact-item"
              ><i class="fas fa-envelope"></i> {{ cv.contact.email }}</span
            >
          </div>
        </div>

        <div class="cv-grid">
          <div class="cv-main-col">
            <div class="cv-group">
              <h4 class="cv-group-title">Perfil Profesional</h4>
              <p class="cv-text">{{ cv.profile }}</p>
            </div>

            <div class="cv-group">
              <h4 class="cv-group-title">Proyectos Destacados</h4>
              <div
                v-for="proj in cv.projects"
                :key="proj.name"
                class="cv-project-item"
              >
                <h5 class="cv-item-title">{{ proj.name }}</h5>
                <span class="cv-item-subtitle">{{ proj.role }}</span>
                <ul class="cv-list">
                  <li v-for="ach in proj.achievements" :key="ach">
                    {{ ach }}
                  </li>
                </ul>
              </div>
            </div>

            <div class="cv-group">
              <h4 class="cv-group-title">Competencias Transversales</h4>
              <div
                v-for="comp in cv.competencies"
                :key="comp.title"
                class="cv-comp-item"
              >
                <strong>{{ comp.title }}:</strong> {{ comp.description }}
              </div>
            </div>
          </div>

          <div class="cv-side-col">
            <div class="cv-group">
              <h4 class="cv-group-title">Habilidades Técnicas</h4>
              <div
                v-for="skill in cv.skills"
                :key="skill.category"
                class="cv-skill-cat"
              >
                <h5>{{ skill.category }}</h5>
                <div class="cv-skill-tags">
                  <span
                    v-for="item in skill.items"
                    :key="item"
                    class="cv-skill-tag"
                    >{{ item }}</span
                  >
                </div>
              </div>
            </div>

            <div class="cv-group">
              <h4 class="cv-group-title">Formación Académica</h4>
              <div
                v-for="edu in cv.education"
                :key="edu.degree"
                class="cv-edu-item"
              >
                <h5 class="cv-item-title">{{ edu.degree }}</h5>
                <p class="cv-item-subtitle">
                  {{ edu.institution }} | {{ edu.year }}
                </p>
                <p class="cv-text-small">{{ edu.description }}</p>
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
  cv: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
/* no additional styles; section uses global rules */
</style>
