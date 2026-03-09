<script setup>
import { ref } from "vue";
import NavBar from "./components/NavBar.vue";
import HeroSection from "./components/HeroSection.vue";
import AboutSection from "./components/AboutSection.vue";
import WorkSection from "./components/WorkSection.vue";
import StatsSection from "./components/StatsSection.vue";
import CaseStudy from "./components/CaseStudy.vue";
import FooterSimple from "./components/FooterSimple.vue";

const projects = ref([
  {
    id: 1,
    title: "EcoMarket",
    description:
      "Showcase de Productos Digitales con Vue.js. Arquitectura SPA con componentes reutilizables, estados reactivos y localización completa para el mercado chileno (CLP/Español). Diseño premium con Glassmorphism.",
    tags: ["Vue.js", "Composition API", "Scoped CSS", "Responsive Design"],
    image: "/img/EcoMarket.png",
    liveUrl:
      "https://valentinapazllr-ops.github.io/analisis-de-caso-Ecomarket/",
    repoUrl:
      "https://github.com/valentinapazllr-ops/analisis-de-caso-Ecomarket",
  },
  {
    id: 2,
    title: "LibroApp",
    description:
      "Gestión de Catálogo Educativo. CRUD completo con integración de Firebase Firestore. Filtrado avanzado y experiencia de usuario fluida con arquitectura de datos escalable.",
    tags: ["Vue.js", "Firebase", "CRUD", "Firestore"],
    image: "/img/LibroApp.png",
    liveUrl: "https://m6-abp.vercel.app/login",
    repoUrl: "https://github.com/valentinapazllr-ops/M6-ABP",
  },
  {
    id: 3,
    title: "SmartBudget",
    description:
      "Aplicación de Presupuesto Personal. Arquitectura moderna para gestión financiera personal, orientada al mercado global con diseño intuitivo.",
    tags: ["Vue.js", "JavaScript", "CSS3"],
    image: "/img/SmartBudget.png",
    liveUrl: "#",
    repoUrl: "#",
  },
  {
    id: 4,
    title: "Alkemi Wallet",
    description:
      "Mi primer proyecto de desarrollo. Aplicación web desarrollada desde cero aplicando fundamentos de HTML, CSS y JavaScript con control de versiones profesional.",
    tags: ["HTML", "CSS", "JavaScript", "Git", "GitHub"],
    image: "/img/AlkemiWallet1.png",
    liveUrl: "https://valentinapazllr-ops.github.io/alke-wallet1-deployment/",
    repoUrl: "https://github.com/valentinapazllr-ops/alke-wallet1",
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

const contactInfo = {
  email: "valentinapazll.r@gmail.com",
  linkedin:
    "https://www.linkedin.com/in/valentina-paz-llantén-robles-a2684a276/",
  github: "https://github.com/valentinapazllr-ops",
};
</script>

<template>
  <div class="app-layout">
    <NavBar :contact="contactInfo" />

    <HeroSection />

    <AboutSection />

    <WorkSection :projects="projects" />

    <CaseStudy v-if="false" :caseStudy="caseStudy" />

    <StatsSection />

    <FooterSimple />
  </div>
</template>
