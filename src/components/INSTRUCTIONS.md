# INSTRUCTIONS — src/components

Propósito
- Contiene componentes reutilizables Astro que forman las secciones del sitio (Hero, Header, Footer, OurServices, Portfolio, etc.).

Estructura y convención
- Cada subcarpeta contiene al menos un archivo `.astro` y opcionalmente un archivo CSS local (p.ej. `hero.css`).
- Nombres: usa PascalCase para archivos `.astro` y kebab/camel para hojas de estilo según la carpeta existente.

Componentes principales en este repo
- `AboutUs` — sección "Sobre nosotros".
- `Background-image` — componente de imagen/hero de fondo.
- `Footer`, `Header` — elementos globales.
- `Hero` — portada principal con CTA.
- `OurServices`, `Portfolio`, `PortfolioGalleryPage`, `VisitUs`, `LinkWhatsapp`.

Consideraciones al editar
- Evitar cambios globales en `global.css` salvo que sea necesario.
- Para cambios visuales, indica el componente exacto y proporciona el mock o el texto.
- Mantener la separación de responsabilidad: lógica mínima en componentes, contenido en páginas.

Pruebas y comprobación rápida
- Levantar con `pnpm dev` y revisar la ruta correspondiente (`/`, `/portfolio`).
