# Copilot / AI Instructions para este repositorio

Resumen rápido
- Proyecto: sitio web estático construido con Astro + Tailwind CSS.
- Estructura clave: `src/components`, `src/layouts`, `src/pages`, `src/styles`, `public`.
- Objetivo de estos archivos: dar contexto estático que la IA puede cargar rápidamente para ahorrar tokens y acelerar cambios.

Stack y comandos
- Tecnologías: Astro, Tailwind, PNPM.
- Comandos habituales:
  - `pnpm install`
  - `pnpm dev` — arranca servidor de desarrollo
  - `pnpm build` — construye para producción

Convenciones de código
- Componentes en `src/components/*` son componentes Astro con CSS local en la misma carpeta.
- Nombres de archivos: PascalCase para componentes (p.ej. `Hero.astro`), kebab o camel para CSS según carpeta.
- Estilos globales en `src/styles/global.css`.

Cómo pedirme cambios (plantilla que ahorra tokens)
Cuando pidas una modificación, incluye exactamente lo siguiente:
1. Objetivo claro (1-2 frases).
2. Archivos afectados o componente por nombre (p.ej. `src/components/Hero/Hero.astro`).
3. Fragmento de código relevante o descripción del cambio; si es mucho, apunta líneas concretas o sube sólo el archivo cambiado.
4. Comportamiento esperado y criterios de aceptación (p.ej. visual, accesibilidad, texto exacto).
5. Comandos/local testing que quieres que use (opcional).

Ejemplo de prompt eficiente:
"Cambiar el botón principal en `src/components/Hero/Hero.astro` para usar clase `btn-primary`, deslizar icono a la izquierda y texto 'Contactar'. Mantener estilos responsivos. Devuélveme sólo el diff del archivo." 

Reglas para la IA al generar respuestas o parches
- Devuelve parches `apply_patch` cuando modifiques archivos.
- Si el cambio afecta a más de 3 archivos, sugiere dividir en PRs pequeños.
- Prefiere cambios locales y puntuales; no reescribir archivos no relacionados.

Archivos de contexto disponibles
- [src/components/INSTRUCTIONS.md](src/components/INSTRUCTIONS.md)
- [src/layouts/INSTRUCTIONS.md](src/layouts/INSTRUCTIONS.md)
- [src/pages/INSTRUCTIONS.md](src/pages/INSTRUCTIONS.md)
- [src/styles/INSTRUCTIONS.md](src/styles/INSTRUCTIONS.md)
- [public/INSTRUCTIONS.md](public/INSTRUCTIONS.md)
- [project.INSTRUCTIONS.md](project.INSTRUCTIONS.md)

Buenas prácticas para ahorrar tokens
- Referencia los archivos por ruta en vez de pegar todo su contenido.
- Si necesitas contexto adicional, pide sólo los bloques concretos (líneas o funciones).
- Usa estos `INSTRUCTIONS.md` como primer lugar de consulta: contienen resúmenes y decisiones de diseño.

Feedback y mantenimiento
- Actualiza estos archivos cuando agregues nuevas carpetas, herramientas o cambies convenciones.

---
Versión: 2026-05-14
