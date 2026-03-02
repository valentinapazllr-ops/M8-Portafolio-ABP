# Portafolio Vue 3 + Vite de Valentina Paz

Este repositorio contiene la aplicación de portafolio personal desarrollada con **Vue 3** y **Vite**.
El objetivo es presentar proyectos, análisis profesionales y documentación estratégica en una SPA moderna con estética "glassmorphism".

### Tecnologías principales
- Vue 3 (Composition API & `<script setup>`)
- Vite como bundler/development server
- CSS moderno con variables, animaciones y diseño responsivo
- FontAwesome para iconografía

## Características de la aplicación
- Navegación fija con enlaces a secciones internas
- Secciones convertidas en componentes reutilizables
- Matriz FODA, case study y CV interactivo
- Descarga de documentos generados en el módulo de empleabilidad
- Estilos centralizados en `src/style.css` con tokens de color

## Estructura del proyecto
```
src/
 ├─ assets/         # imágenes y recursos estáticos
 ├─ components/     # componentes Vue desglosados
 ├─ App.vue         # punto de entrada de la UI
 ├─ main.js         # bootstrap de la app
 ├─ style.css       # estilos globales y variables
 public/docs/       # documentación entregada (markdown)
```

## Instalar y ejecutar

```bash
npm install       # instala dependencias
npm run dev       # levanta servidor de desarrollo (http://localhost:3000)
npm run build     # genera versión de producción
npm run preview   # previsualiza el build
```

## Despliegue
El proyecto incluye un script `npm run deploy` que construye el sitio y sube la carpeta `dist` a [GitHub Pages](https://pages.github.com/) usando `gh-pages`.

## Personalización
- Cambia los datos del currículum y los proyectos en `src/App.vue`.
- Añade nuevas secciones creando componentes bajo `src/components` y registrándolos en App.
- Modifica colores y tipografías editando `:root` en `src/style.css`.

## Archivos generados
- [ linkedin_optimization.md ](./public/docs/linkedin_optimization.md)
- [ elevator_pitch.md ](./public/docs/elevator_pitch.md)
- [ linkedin_post.md ](./public/docs/linkedin_post.md)
- [ final_delivery.md ](./public/docs/final_delivery.md)

---
*Este README fue mejorado para brindar más contexto y facilitar el uso del portafolio web.*