**Plan de Modernización — Proyecto Maestría del Hierro**

**Resumen:**: Plan estratégico para modernizar la web, mejorar percepción profesional, optimizar performance y añadir funcionalidades visuales de alto impacto (hero llamativo, galería, animaciones y mejoras UX/SEO).

**Objetivos Principales:**
- **Impacto visual:**: Crear un `Hero` inicial profesional y llamativo que refleje la calidad artesanal.
- **Portafolio atractivo:**: Mostrar muchos más detalles fotográficos en una galería filtrable con lightbox.
- **Percepción profesional:**: Mejorar tipografía, paleta y microinteracciones para transmitir confianza.
- **Performance & SEO:**: Mantener tiempos de carga bajos y buenas métricas Lighthouse.

**Alcance:**
- Componentes a actualizar: [src/components/Hero/Hero.astro](src/components/Hero/Hero.astro#L1), [src/components/Portfolio/Portfolio.astro](src/components/Portfolio/Portfolio.astro#L1), [src/components/linkWhatsapp/LinkWhatsapp.astro](src/components/linkWhatsapp/LinkWhatsapp.astro#L1).
- Archivos globales: [src/styles/global.css](src/styles/global.css#L1), `package.json` (dependencias opcionales para Lottie o tiny libraries).
- Nuevos componentes sugeridos: `src/components/Gallery/Gallery.astro`, `src/components/CaseStudy/CaseStudy.astro`.

**Entregables:**
- **Hero rediseñado**: `Hero.astro` + estilos y assets optimizados.
- **Galería/Portfolio**: componente `Gallery` con masonry y lightbox.
- **Tokens de diseño**: actualización en `global.css` (colores, tipografías, keyframes).
- **Guía breve**: `README_MODERNIZACION.md` con pasos de despliegue y pruebas.

**Prioridades (primer sprint):**
1. Rediseño del `Hero` (visual impacto inmediato).
2. Migrar y optimizar imágenes clave (WebP/AVIF, `srcset`).
3. Implementar galería filtrable con lightbox.
4. Añadir animaciones sutiles y Lottie en CTA.

**Tareas y pasos detallados:**
- **1 — Auditoría de activos**: inventario de fotos, tamaños y metadatos; identificar imágenes a convertir a WebP/AVIF.
- **2 — Diseño del Hero**:
  - Elegir imagen principal de alta calidad (o composite con textura SVG).
  - Implementar overlay con gradiente + textura sutil.
  - Texto en dos líneas con reveal animation y CTA destacado (botón accesible).
  - Parallax ligero opcional en background.
- **3 — Sistema de imágenes**:
  - Generar versiones 320/640/1024/1600 en WebP/AVIF.
  - Usar `picture` + `source` + `loading="lazy"` + `decoding="async"`.
- **4 — Galería/Portfolio**:
  - Grid masonry responsivo con filtro por categoría.
  - Lightbox accesible (focus trap, teclado, swipe en móvil).
- **5 — Tipografía & Paleta**:
  - Seleccionar 1 serif elegante para títulos y 1 sans para cuerpo.
  - Definir variables CSS: `--accent`, `--muted`, `--bg`, `--text`.
- **6 — Animaciones y microinteracciones**:
  - Keyframes para reveal, pulse en CTA, hover elevación en cards.
  - IntersectionObserver para entradas lazy-animate.
  - Integrar 1–2 animaciones Lottie optimizadas.
- **7 — SVG y detalles ornamentales**:
  - SVGs inline para ornamentos con animación CSS leve.
- **8 — Accesibilidad y SEO**:
  - ALT completos, roles ARIA donde aplique, metadatos OG y JSON-LD para proyectos.
- **9 — Performance**:
  - Critical CSS, carga diferida de scripts, preconnect a CDN/fonts, medir con Lighthouse.

**Criterios de aceptación (mínimos):**
- `Hero`: carga responsable en móvil, CTA visible y animación sin jank.
- `Gallery`: filtros funcionales y lightbox usable con teclado.
- Lighthouse (mobile): Performance ≥ 85, Accessibility ≥ 90 (meta inicial).
- Imágenes: servidas en WebP/AVIF con `srcset` y lazy-loading.

**Recomendaciones técnicas y librerías (opcional):**
- `lazysizes` o usar nativo `loading="lazy"` (preferible nativo).
- `lottie-web` para animaciones vectoriales ligeras (usar JSON optimizado).
- `micromodal` o implementación propia para lightbox accesible mínima.
- Evitar librerías UI pesadas; preferir utilidades CSS y pequeñas librerías específicas.

**Pruebas y despliegue:**
- Probar en móviles (iPhone/Android), tablet y desktop con herramientas de responsive.
- Ejecutar Lighthouse en modo incognito y ajustar.
- Comandos básicos para test local:

```bash
pnpm install
pnpm dev
pnpm build
pnpm preview
```

**Timeline estimado (iteración 1 — 2 semanas):**
- Días 1–2: Auditoría de imágenes y selección de assets.
- Días 3–5: Rediseño e implementación del `Hero` + estilos globales.
- Días 6–9: Implementación de galería y lightbox.
- Días 10–12: Animaciones, Lottie y ajuste fino.
- Día 13–14: Tests, optimizaciones de performance y entrega.

**Siguientes pasos:**
- Confirmame si quieres que implemente ahora el `Hero` y `global.css` (entregando diffs), o prefieres que empiece por la galería.

---
Versión: 2026-05-14
