<script setup>
import { ref } from "vue";
import NavBar from "./components/NavBar.vue";
import HeroSection from "./components/HeroSection.vue";
import WorkSection from "./components/WorkSection.vue";
import CaseStudy from "./components/CaseStudy.vue";
import FodaSection from "./components/FodaSection.vue";
import CVSection from "./components/CVSection.vue";
import DocsSection from "./components/DocsSection.vue";
import FooterSimple from "./components/FooterSimple.vue";

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
    <NavBar :contact="cv.contact" />

    <HeroSection />

    <WorkSection :projects="projects" />

    <CaseStudy :caseStudy="caseStudy" />

    <FodaSection :foda="foda" />

    <CVSection :cv="cv" />

    <DocsSection :docs="docs" />

    <FooterSimple />
  </div>
</template>

