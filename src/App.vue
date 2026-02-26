<script setup>
import { ref } from "vue";

const projects = ref([
  {
    id: 1,
    title: "EcoMarket",
    description:
      "Showcase de Productos Digitales con Vue.js. Optimización de renderizado y localización.",
    tags: ["Vue.js", "Props", "Lifecycle Hooks"],
    image: "src/assets/img/ecoMarket.png",
  },
  {
    id: 2,
    title: "LibroApp",
    description:
      "Gestión de Catálogo Educativo con CRUD completo e integración de Firebase.",
    tags: ["Vue.js", "Firebase", "CRUD"],
    image: "src/assets/img/libroApp.png",
  },
  {
    id: 3,
    title: "Alkemi WAllet 1",
    description: "Es el primer proyecto que desarrolle en clases.",
    tags: ["HTML", "CSS", "JS", "Git", "GitHub", "VSCode"],
    image: "src/assets/img/AlkemiWallet1.png",
  },
  {
    id: 4,
    title: "SmartBudget",
    description:
      "Aplicación de presupuesto personal con arquitectura moderna para el mercado global.",
    tags: ["HTML", "CSS", "Js", "SCSS", "Git", "GitHub", "VSCode"],
    image: "src/assets/img/SmartBudget.png",
  },
]);

const caseStudy = ref({
  title: "EcoMarket Architecture",
  challenge:
    "La arquitectura basada en componentes permitió transformar una interfaz rígida en un sistema modular escalable. El mayor desafío fue asegurar que cada pieza del puzzle fuera independiente pero perfectamente sincronizada.",
  solution:
    "Implementé una jerarquía de componentes clara, facilitando que el desarrollo de nuevas funcionalidades sea reactivo y eficiente, minimizando la duplicidad de estilos y lógica.",
  details: [
    {
      title: "Modularidad Total",
      items: ["NavBar Dinámica", "ProductCard con Props", "BaseCard Template"],
    },
    {
      title: "Arquitectura Vue",
      items: [
        "Jerarquía Root/Vista/Hijo",
        "Eventos Personalizados",
        "Slots para Reusabilidad",
      ],
    },
    {
      title: "Optimización UX",
      items: [
        "onMounted para Data Fetching",
        "onUnmounted para Perf",
        "Dynamic Components",
      ],
    },
    {
      title: "Diseño Técnico",
      items: ["Class/Style Binding", "Scoped CSS", "Global Theme Tokens"],
    },
  ],
  justification:
    "Este proyecto es el pilar de mi portafolio porque demuestra solidez técnica y una visión estratégica del desarrollo de producto.",
});

const foda = ref({
  fortalezas: [
    "Dominio de Vue.js 3",
    "Diseño UI/UX Sophisticated",
    "Metodologías Ágiles",
    "Resolución de Problemas",
    "Colaboración Técnica",
  ],
  debilidades: [
    "Inglés C1 (Proceso)",
    "Back-End Nativo",
    "Cloud Infraestructure",
    "Unit Testing Avanzado",
    "CI/CD Pipelines",
  ],
  oportunidades: [
    "Mercado Dev Remoto",
    "Ecosistema Vue LATAM",
    "Transformación Digital",
    "Soluciones ERP Modernas",
    "Networking Estratégico",
  ],
  amenazas: [
    "Saturación de Mercado",
    "Evolución de Motores IA",
    "Contexto Económico",
    "Nuevos Frameworks",
    "Competencia Global",
  ],
});

const docs = ref([
  {
    name: "linkedin_optimization.md",
    url: "/docs/linkedin_optimization.md",
    icon: "fab fa-linkedin",
  },
  {
    name: "elevator_pitch.md",
    url: "/docs/elevator_pitch.md",
    icon: "fas fa-microphone-alt",
  },
  {
    name: "linkedin_post.md",
    url: "/docs/linkedin_post.md",
    icon: "fas fa-share-alt",
  },
  {
    name: "final_delivery.md",
    url: "/docs/final_delivery.md",
    icon: "fas fa-file-export",
  },
]);

const cv = ref({
  name: "VALENTINA PAZ LLANTÉN ROBLES",
  title:
    "Junior Full Stack Developer | Especialista en Vue.js & Soluciones Digitales",
  location: "Santiago, Chile (Disponible para Remoto)",
  contact: {
    email: "valentinapazll.r@gmail.com",
    linkedin: "https://www.linkedin.com/in/valentina-llantén-robles-a2684a276/",
    github: "https://github.com/valentinapazllr-ops",
  },
  profile:
    "Desarrolladora Full Stack Junior con un fuerte enfoque en el ecosistema Frontend modern (Vue.js) y pasión por la creación de interfaces intuitivas y de alto impacto visual. Experiencia técnica en el desarrollo de SPAs dinámicas, gestión de datos con Firebase y metodologías ágiles. Me distingo por mi capacidad analítica para resolver problemas complejos, mi adaptabilidad ante nuevas tecnologías y un compromiso inquebrantable con la calidad del código y la experiencia del usuario (UX).",
  skills: [
    {
      category: "Frontend",
      items: [
        "Vue.js (Composition API)",
        "JavaScript (ES6+)",
        "HTML5",
        "CSS3 (Glassmorphism, Gradients)",
        "Responsive Design",
      ],
    },
    {
      category: "Backend & Tools",
      items: ["Firebase (Firestore)", "VSCode", "Java", "Git", "GitHub"],
    },
    {
      category: "Soft Skills",
      items: [
        "Comunicación asertiva",
        "Trabajo en equipo multidisciplinar",
        "Resolución proactiva de problemas",
        "Aprendizaje continuo",
      ],
    },
    { category: "Idiomas", items: ["Español (Nativo)", "Inglés (Técnico)"] },
  ],
  projects: [
    {
      name: "EcoMarket – Showcase de Productos Digitales",
      role: "Desarrolladora Frontend",
      achievements: [
        "Arquitecté una Single Page Application (SPA) utilizando Vue.js, priorizando la modularización mediante componentes reutilizables.",
        "Optimicé el rendimiento mediante la gestión eficiente del ciclo de vida de componentes y estados reactivos.",
        'Implementé una interfaz "Premium" con estéticas modernas, asegurando una localización completa (CLP/Español) para el mercado regional.',
      ],
    },
    {
      name: "LibroApp – Gestión de Inventario Educativo",
      role: "Desarrolladora De Aplicaciones Frontend Trainee",
      achievements: [
        "Desarrollé un sistema CRUD completo para la administración de catálogos, integrando lógica de negocio y persistencia de datos eficientemente.",
        "Diseñé una experiencia de usuario fluida con sistemas de filtrado avanzados y una estética visual coherente y profesional.",
        "Colaboré en la definición de la arquitectura de datos para asegurar la escalabilidad del proyecto.",
      ],
    },
  ],
  education: {
    degree: "Certificación en Desarrollo de Aplicaciones Front-end Trainee",
    institution: "Sence- Instituto ISEG",
    year: "2026",
    description:
      "Formación intensiva con foco en arquitectura de software, metodologías ágiles y desarrollo de producto.",
  },
  competencies: [
    {
      title: "Liderazgo Técnico",
      description:
        "Proactividad en la documentación de procesos técnicos, facilitando la integración de nuevos miembros al equipo.",
    },
    {
      title: "Eficiencia Operativa",
      description:
        "Automatización de flujos de prueba en proyectos académicos, mejorando la detección temprana de bugs.",
    },
    {
      title: "Visión de Producto",
      description:
        "Capacidad para alinear decisiones técnicas con los objetivos de negocio y las necesidades del usuario final.",
    },
  ],
});
</script>

<template>
  <div class="app-layout">
    <!-- Sophisticated Header -->
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
              href="https://www.linkedin.com/in/valentina-llant%C3%A9n-robles-a2684a276/"
              target="_blank"
              ><i class="fab fa-linkedin-in"></i
            ></a>
            <a href="https://github.com/valentinapazllr-ops" target="_blank"
              ><i class="fab fa-github"></i
            ></a>
            <a href="mailto:valentinapazll.r@gmail.com" class="btn-email"
              >Contact</a
            >
          </div>
        </div>
      </div>
    </nav>

    <!-- Refined Hero -->
    <header class="hero-section animate-reveal">
      <div class="premium-container hero-grid">
        <div class="hero-content">
          <div class="badge-new">2026 Portfolio</div>
          <h1 class="hero-main-title">
            Valentina Paz <br /><span class="gradient-text"
              >Llantén Robles</span
            >
          </h1>
          <p class="hero-lead">
            Junior Tech Talent & Front-End Developer Trainee.
          </p>
          <p class="hero-story">
            Convierto ideas complejas en interfaces dinámicas de alto
            rendimiento utilizando Vue.js y los estándares más modernos del
            ecosistema web.
          </p>
          <div class="tech-stack">
            <span class="tech-tag"><i class="fab fa-vuejs"></i> Vue 3</span>
            <span class="tech-tag"><i class="fab fa-js"></i> JavaScript</span>
            <span class="tech-tag"><i class="fas fa-fire"></i> Firebase</span>
            <span class="tech-tag"><i class="fas fa-code"></i> VS Code</span>
          </div>
        </div>
      </div>
    </header>

    <!-- Work Section -->
    <section id="proyectos" class="section work-section">
      <div class="premium-container">
        <div class="section-header">
          <h2 class="title-xl">
            Featured <span class="gradient-text">Work</span>
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
                  @error="
                    (e) =>
                      (e.target.src =
                        'https://via.placeholder.com/600x400?text=Work')
                  "
                />
              </div>
              <div class="project-info">
                <h3 class="p-title">{{ p.title }}</h3>
                <p class="p-desc">{{ p.description }}</p>
                <div class="p-tags">
                  <span v-for="tag in p.tags" :key="tag" class="tag-pill">{{
                    tag
                  }}</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Case Study Overhaul -->
    <section id="estudio" class="section case-section">
      <div class="premium-container">
        <div class="glass-card case-outer animate-reveal">
          <div class="case-columns">
            <div class="case-main">
              <span class="case-label">Case Study #01</span>
              <h2 class="case-title">{{ caseStudy.title }}</h2>
              <div class="case-intro">
                <div class="intro-block">
                  <h4>Desafío</h4>
                  <p>{{ caseStudy.challenge }}</p>
                </div>
                <div class="intro-block">
                  <h4>Solución</h4>
                  <p>{{ caseStudy.solution }}</p>
                </div>
              </div>
              <div class="case-quote">
                <p>{{ caseStudy.justification }}</p>
              </div>
            </div>
            <div class="case-sidebar">
              <div
                v-for="detail in caseStudy.details"
                :key="detail.title"
                class="sidebar-item"
              >
                <h5>{{ detail.title }}</h5>
                <ul>
                  <li v-for="item in detail.items" :key="item">{{ item }}</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Strategic Analysis -->
    <section id="foda" class="section foda-section">
      <div class="premium-container">
        <div class="section-header">
          <h2 class="title-xl">
            Strategic <span class="gradient-text">Analysis</span>
          </h2>
          <p class="section-subtitle">
            Matriz FODA aplicada al perfil profesional IT.
          </p>
        </div>
        <div class="foda-quadrants">
          <div class="foda-q glass-card green-q animate-reveal">
            <div class="q-header">
              <i class="fas fa-arrow-up"></i> Fortalezas
            </div>
            <ul>
              <li v-for="item in foda.fortalezas" :key="item">{{ item }}</li>
            </ul>
          </div>
          <div class="foda-q glass-card blue-q animate-reveal">
            <div class="q-header">
              <i class="fas fa-star"></i> Oportunidades
            </div>
            <ul>
              <li v-for="item in foda.oportunidades" :key="item">{{ item }}</li>
            </ul>
          </div>
          <div class="foda-q glass-card red-q animate-reveal">
            <div class="q-header">
              <i class="fas fa-exclamation-triangle"></i> Debilidades
            </div>
            <ul>
              <li v-for="item in foda.debilidades" :key="item">{{ item }}</li>
            </ul>
          </div>
          <div class="foda-q glass-card orange-q animate-reveal">
            <div class="q-header">
              <i class="fas fa-shield-alt"></i> Amenazas
            </div>
            <ul>
              <li v-for="item in foda.amenazas" :key="item">{{ item }}</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- CV Section -->
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
                <div class="cv-edu-item">
                  <h5 class="cv-item-title">{{ cv.education.degree }}</h5>
                  <p class="cv-item-subtitle">
                    {{ cv.education.institution }} | {{ cv.education.year }}
                  </p>
                  <p class="cv-text-small">{{ cv.education.description }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Generated Files Section -->
    <section id="archivos" class="section docs-section">
      <div class="premium-container">
        <div class="section-header">
          <h2 class="title-xl">
            Archivos <span class="gradient-text">Generados</span>
          </h2>
          <p class="section-subtitle">
            Documentación estratégica y entregables del módulo de empleabilidad.
          </p>
        </div>
        <div class="docs-grid">
          <a
            v-for="doc in docs"
            :key="doc.name"
            :href="doc.url"
            target="_blank"
            class="glass-card doc-card animate-reveal"
          >
            <div class="doc-icon">
              <i :class="doc.icon"></i>
            </div>
            <div class="doc-info">
              <span class="doc-name">{{ doc.name }}</span>
              <span class="doc-action"
                >Abrir archivo <i class="fas fa-external-link-alt"></i
              ></span>
            </div>
          </a>
        </div>
      </div>
    </section>

    <footer class="footer-simple">
      <div class="premium-container">
        <div class="footer-wrap">
          <span class="footer-logo">Valentina.</span>
          <p class="copyright">
            © 2026 Developed with passion for the digital future.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<style>
/* Reset & Base */
.app-layout {
  padding-top: 100px;
}

/* Navbar */
.main-nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 100px;
  z-index: 2000;
  background: rgba(10, 15, 22, 0.8);
  -webkit-backdrop-filter: blur(15px);
  backdrop-filter: blur(15px);
  border-bottom: 1px solid var(--glass-border);
}

.nav-inner {
  height: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.8rem;
  font-weight: 800;
  cursor: pointer;
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 2.5rem;
}
.nav-links a {
  text-decoration: none;
  color: var(--text-secondary);
  font-weight: 600;
  font-size: 0.95rem;
  transition: color 0.3s ease;
}
.nav-links a:hover {
  color: var(--text-primary);
}

.nav-divider {
  width: 1px;
  height: 30px;
  background: var(--glass-border);
}

.social-box {
  display: flex;
  align-items: center;
  gap: 1.2rem;
}
.social-box a {
  font-size: 1.1rem;
}
.social-box a:hover {
  color: var(--accent-primary);
}

.btn-email {
  background: var(--premium-gradient);
  color: white !important;
  padding: 0.6rem 1.8rem;
  border-radius: 99px;
  font-size: 0.9rem !important;
  transition: transform 0.3s ease !important;
}
.btn-email:hover {
  transform: translateY(-2px);
}

/* Hero */
.hero-section {
  padding: 10rem 0 8rem;
}
.hero-grid {
  text-align: left;
}
.hero-content {
  max-width: 800px;
}

.badge-new {
  display: inline-block;
  padding: 0.4rem 1rem;
  background: rgba(16, 185, 129, 0.1);
  color: var(--accent-primary);
  border-radius: 12px;
  font-weight: 700;
  margin-bottom: 1.5rem;
  font-size: 0.85rem;
  border: 1px solid rgba(16, 185, 129, 0.2);
}

.hero-main-title {
  font-size: 5.5rem;
  line-height: 1;
  font-weight: 800;
  margin-bottom: 2rem;
}
.hero-lead {
  font-size: 1.8rem;
  color: var(--text-primary);
  font-weight: 400;
  margin-bottom: 1rem;
}
.hero-story {
  font-size: 1.2rem;
  color: var(--text-secondary);
  margin-bottom: 3rem;
  max-width: 600px;
  line-height: 1.8;
}

.tech-stack {
  display: flex;
  gap: 1.2rem;
  flex-wrap: wrap;
}
.tech-tag {
  background: var(--glass-bg);
  padding: 0.8rem 1.5rem;
  border-radius: 20px;
  border: 1px solid var(--glass-border);
  font-size: 0.95rem;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 0.6rem;
}
.tech-tag i {
  color: var(--accent-primary);
}

/* Work Section */
.section-header {
  margin-bottom: 5rem;
  text-align: left;
}
.title-xl {
  font-size: 3.5rem;
  font-weight: 800;
  margin-bottom: 1rem;
}
.section-subtitle {
  font-size: 1.2rem;
  color: var(--text-secondary);
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
  gap: 3rem;
}
.project-card {
  padding: 0;
  overflow: hidden;
  height: 100%;
  display: flex;
  flex-direction: column;
}

.img-container {
  width: 100%;
  height: 260px;
  overflow: hidden;
}
.project-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.6s ease;
}
.project-card:hover .project-img {
  transform: scale(1.1);
}

.project-info {
  padding: 2.5rem;
  flex-grow: 1;
  display: flex;
  flex-direction: column;
}
.p-title {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}
.p-desc {
  color: var(--text-secondary);
  margin-bottom: 2rem;
  flex-grow: 1;
}
.p-tags {
  display: flex;
  gap: 0.8rem;
  flex-wrap: wrap;
}
.tag-pill {
  padding: 0.4rem 1rem;
  border-radius: 10px;
  background: rgba(255, 255, 255, 0.05);
  font-size: 0.8rem;
  font-weight: 700;
  color: var(--accent-primary);
  border: 1px solid var(--glass-border);
}

/* Case Study Section */
.case-section {
  background: rgba(255, 255, 255, 0.01);
}
.case-outer {
  padding: 5rem;
}
.case-columns {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 6rem;
}

.case-label {
  display: block;
  color: var(--accent-primary);
  font-weight: 800;
  font-size: 0.8rem;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
  letter-spacing: 0.2rem;
}
.case-title {
  font-size: 3.5rem;
  font-weight: 800;
  margin-bottom: 3rem;
  line-height: 1;
}

.case-intro {
  display: grid;
  gap: 2.5rem;
  margin-bottom: 3.5rem;
}
.intro-block h4 {
  font-size: 1.1rem;
  margin-bottom: 1rem;
  color: var(--text-primary);
}
.intro-block p {
  color: var(--text-secondary);
  font-size: 1.05rem;
}

.case-quote {
  padding: 2.5rem;
  border-left: 2px solid var(--accent-primary);
  background: rgba(16, 185, 129, 0.03);
  color: #82f1ce;
  font-size: 1.1rem;
  font-style: italic;
}

.case-sidebar {
  display: grid;
  gap: 2.5rem;
}
.sidebar-item h5 {
  font-size: 1rem;
  color: var(--accent-primary);
  margin-bottom: 1.2rem;
}
.sidebar-item ul {
  list-style: none;
  padding: 0;
}
.sidebar-item li {
  font-size: 0.95rem;
  color: var(--text-secondary);
  padding: 0.8rem 0;
  border-bottom: 1px solid var(--glass-border);
}

/* FODA Section */
.foda-quadrants {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}
.foda-q {
  padding: 3rem;
}
.q-header {
  display: flex;
  align-items: center;
  gap: 0.8rem;
  font-size: 1.2rem;
  font-weight: 800;
  margin-bottom: 2rem;
  text-transform: uppercase;
  border-bottom: 1px solid var(--glass-border);
  padding-bottom: 1rem;
}

.foda-q ul {
  list-style: none;
}
.foda-q li {
  color: var(--text-secondary);
  margin-bottom: 1rem;
  font-size: 1rem;
  padding-left: 1.5rem;
  position: relative;
}
.foda-q li::before {
  content: "•";
  position: absolute;
  left: 0;
  color: var(--accent-primary);
}

.green-q .q-header {
  color: #10b981;
}
.blue-q .q-header {
  color: #3b82f6;
}
.red-q .q-header {
  color: #ef4444;
}
.orange-q .q-header {
  color: #f59e0b;
}

/* CV Section Styling */
.cv-container {
  padding: 4rem;
  background: rgba(255, 255, 255, 0.02);
}

.cv-header-info {
  text-align: center;
  margin-bottom: 4rem;
  border-bottom: 1px solid var(--glass-border);
  padding-bottom: 3rem;
}

.cv-name {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
}

.cv-tagline {
  font-size: 1.1rem;
  color: var(--accent-primary);
  font-weight: 600;
  margin-bottom: 1.5rem;
}

.cv-contact-row {
  display: flex;
  justify-content: center;
  gap: 2rem;
  color: var(--text-secondary);
  font-size: 0.9rem;
}

.cv-contact-item i {
  color: var(--accent-primary);
  margin-right: 0.5rem;
}

.cv-grid {
  display: grid;
  grid-template-columns: 1.8fr 1fr;
  gap: 4rem;
}

.cv-group {
  margin-bottom: 3rem;
}

.cv-group-title {
  font-size: 1.2rem;
  font-weight: 800;
  text-transform: uppercase;
  color: var(--text-primary);
  margin-bottom: 1.5rem;
  display: flex;
  align-items: center;
  gap: 1rem;
}

.cv-group-title::after {
  content: "";
  flex-grow: 1;
  height: 1px;
  background: var(--glass-border);
}

.cv-text {
  color: var(--text-secondary);
  line-height: 1.8;
  font-size: 1rem;
}

.cv-project-item {
  margin-bottom: 2rem;
}

.cv-item-title {
  font-size: 1.2rem;
  font-weight: 700;
  margin-bottom: 0.3rem;
  color: var(--text-primary);
}

.cv-item-subtitle {
  font-size: 0.9rem;
  color: var(--accent-primary);
  font-weight: 600;
  display: block;
  margin-bottom: 1rem;
}

.cv-list {
  padding-left: 1.2rem;
  color: var(--text-secondary);
}

.cv-list li {
  margin-bottom: 0.8rem;
  font-size: 0.95rem;
  line-height: 1.6;
}

.cv-skill-cat {
  margin-bottom: 2rem;
}

.cv-skill-cat h5 {
  font-size: 1rem;
  color: var(--text-primary);
  margin-bottom: 1rem;
}

.cv-skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem;
}

.cv-skill-tag {
  padding: 0.4rem 0.8rem;
  background: rgba(16, 185, 129, 0.05);
  border: 1px solid var(--glass-border);
  border-radius: 6px;
  font-size: 0.85rem;
  color: var(--text-secondary);
}

.cv-comp-item {
  margin-bottom: 1rem;
  font-size: 0.95rem;
  color: var(--text-secondary);
}

.cv-comp-item strong {
  color: var(--text-primary);
}

.cv-text-small {
  font-size: 0.9rem;
  color: var(--text-secondary);
  margin-top: 0.5rem;
}

/* Docs Grid Styling */
.docs-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.doc-card {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  padding: 2rem;
  text-decoration: none;
  transition:
    transform 0.3s ease,
    border-color 0.3s ease !important;
}

.doc-card:hover {
  transform: translateY(-5px);
  border-color: var(--accent-primary) !important;
}

.doc-icon {
  width: 50px;
  height: 50px;
  background: rgba(16, 185, 129, 0.1);
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.5rem;
  color: var(--accent-primary);
  flex-shrink: 0;
}

.doc-info {
  display: flex;
  flex-direction: column;
  gap: 0.3rem;
}

.doc-name {
  font-weight: 700;
  color: var(--text-primary);
  font-size: 1.1rem;
}

.doc-action {
  font-size: 0.8rem;
  color: var(--text-secondary);
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

/* Footer */
.footer-simple {
  padding: 6rem 0;
  border-top: 1px solid var(--glass-border);
}
.footer-wrap {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.footer-logo {
  font-size: 1.5rem;
  font-weight: 800;
}
.copyright {
  color: var(--text-secondary);
  font-size: 0.9rem;
}

@media (max-width: 1024px) {
  .cv-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
  .case-columns {
    grid-template-columns: 1fr;
    gap: 4rem;
  }
  .hero-main-title {
    font-size: 4rem;
  }
  .case-outer {
    padding: 3rem;
  }
  .cv-container {
    padding: 2rem;
  }
}

@media (max-width: 768px) {
  .hero-main-title {
    font-size: 3rem;
  }
  .nav-links {
    display: none;
  }
  .hero-section {
    padding-top: 6rem;
  }
  .cv-contact-row {
    flex-direction: column;
    gap: 0.5rem;
  }
}
</style>
