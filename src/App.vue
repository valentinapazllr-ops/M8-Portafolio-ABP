<script setup>
import { ref } from "vue";
import NavBar from "./components/NavBar.vue";
import HeroSection from "./components/HeroSection.vue";
import WorkSection from "./components/WorkSection.vue";
import CaseStudy from "./components/CaseStudy.vue";
import FodaSection from "./components/FodaSection.vue";
import CVSection from "./components/CVSection.vue";
import FooterSimple from "./components/FooterSimple.vue";

const projects = ref([
  {
    id: 1,
    title: "EcoMarket",
    description:
      "Showcase de Productos Digitales con Vue.js. Optimización de renderizado y localización.",
    tags: ["Vue.js", "Props", "Lifecycle Hooks"],
    image: "/img/EcoMarket.png",
  },
  {
    id: 3,
    title: "Alkemi WAllet 1",
    description: "Es el primer proyecto que desarrolle en clases.",
    tags: ["HTML", "CSS", "JS", "Git", "GitHub", "VSCode"],
    image: "/img/AlkemiWallet1.png",
  },
  {
    id: 4,
    title: "SmartBudget",
    description:
      "Aplicación de presupuesto personal con arquitectura moderna para el mercado global.",
    tags: ["HTML", "CSS", "Js", "SCSS", "Git", "GitHub", "VSCode"],
    image: "/img/SmartBudget.png",
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
  Fortalezas: [
    "Dominio de HTML, CSS y SCSS — Sólida base en maquetación semántica, diseño responsivo y preprocesadores con metodologías como BEM y SCSS modular.",
    "Desarrollo con Vue.js y manejo de estado — Conocimiento aplicado de Vue 3, Vuex y componentes reutilizables, evidenciado en proyectos reales como EcoMarket y LibroApp.",
    "JavaScript moderno (ES6+) — Manejo de conceptos como promesas, async/await, manipulación del DOM, OOP y manejo de eventos.",
    "Gestión de proyectos con Git y GitHub — Uso de control de versiones, flujo de trabajo con ramas, commits y despliegue en GitHub Pages.",
    "Capacidad de aprendizaje autónomo y orientado a proyectos — Formación intensiva en bootcamp con entrega de proyectos ABP aplicados a situaciones reales, con habilidad para buscar soluciones de forma independiente",
  ],
  Debilidades: [
    "Inglés técnico limitado — Leer documentación es posible, pero la comunicación fluida en inglés (escrita y oral) es aún un área a fortalecer, siendo un filtro clave para posiciones remotas internacionales.",
    "Sin experiencia en backend ni Python — No dominas lenguajes de servidor como Python, Node.js o bases de datos relacionales, lo que limita el alcance como desarrolladora full stack real",
    "Experiencia laboral formal aún en construcción — Tus proyectos son académicos; aún no cuentas con experiencia en entornos productivos reales con equipos y deadlines empresariales. ",
    "Testing y calidad de código — Herramientas como Jest, Testing Library o buenas prácticas de QA (unit testing, E2E) son aún poco exploradas en tu formación.",
    "Dominio limitado de herramientas DevOps y despliegue — Conceptos como CI/CD, Docker, o deployment en plataformas como Vercel, Netlify o AWS están fuera de tu stack actual.",
  ],
  Oportunidades: [
    "Alta competencia entre perfiles junior — El mercado tiene un exceso de desarrolladores junior y escasez de seniors; entrar al primer empleo es el mayor obstáculo. ",
    "La IA está automatizando tareas básicas de desarrollo — Herramientas como GitHub Copilot o Cursor están reemplazando código repetitivo, elevando el estándar mínimo esperado de un desarrollador. ",
    "Competencia global en trabajo remoto — Al postular a empleos remotos, compites no solo con profesionales de Santiago, sino con desarrolladores de toda Latinoamérica y el mundo.",
    "Requisito creciente de inglés fluido — Muchas vacantes bien remuneradas (especialmente en nearshoring) requieren inglés conversacional como condición no negociable. ",
    "Mercado más exigente en especialización — Las empresas ya no buscan generalistas; priorizan perfiles con especialización clara (Vue/React avanzado, Next.js, TypeScript, rendimiento web)",
  ],
  Amenazas: [
    "Alta competencia en puestos de nivel Junior",
    "Evolución constante y rápida de tecnologías Web",
    "Ofertas laborales que exigen rol Full-Stack desde el inicio",
  ],
});

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
  education: {
    degree: "Tecnico en Turismo",
    institution: "Instituto Profesional Aiep",
    year: "2013 - 2017",
    description:
      "Estudio Superior tecnico sobre gestión de destinos, hotelería, gastronomía, relaciones públicas y administración de empresas turísticas.",
  },
  education: {
    degree: "Cientifico Humanista - Media",
    institution: "Colegio San Luis Beltran",
    year: "2008 - 2011",
    description: "Termine mi educación media en el area cientifico humanista",
  },
  education: {
    degree: "Enseñanza basica",
    institution: "Colegio Madre Ana Eugenia",
    year: "1999 - 2007",
    description: "Estudie en el colegio Pre- Kinder a 8vo basico",
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

    <FooterSimple />
  </div>
</template>
