 # Copilot / AI Instructions para este repositorio (archivo .github)

Este archivo provee instrucciones claras para asistentes AI que trabajen en el repo.

Resumen rápido
- Proyecto: sitio web estático construido con Astro + Tailwind CSS.
- Estructura clave: `src/components`, `src/layouts`, `src/pages`, `src/styles`, `public`.
- Objetivo: ofrecer contexto y reglas para generar cambios seguros y coherentes.

Uso del cache de contexto (mcp-context-cache)
- Antes de leer archivos grandes o hacer búsquedas, la IA **debe** revisar y usar `contextcache.json` en la raíz del proyecto si existe. Esto acelera el trabajo y reduce uso de tokens.
- Si `contextcache.json` existe, la IA debe cargarlo y seguir la configuración `modules` y `globalInstructions` definida allí.

Stack y comandos
- Tecnologías: Astro, Tailwind, PNPM.
- Comandos habituales:
  - `pnpm install`
  - `pnpm dev` — arranca servidor de desarrollo
  - `pnpm build` — construye para producción

Convenciones de código
- Componentes en `src/components/*` son componentes Astro con CSS local en la misma carpeta.
- Nombres de archivos: PascalCase para componentes (p.ej. `Hero.astro`).
- Estilos globales en `src/styles/global.css`.

Reglas estrictas para herramientas y acceso a archivos
- NO usar las herramientas `read_file`, `list_dir`, `file_search`, `semantic_search` ni `grep_search` directamente al inicio de una tarea cuando `contextcache.json` existe.
- Si el `mcp-context-cache` está disponible y contiene la configuración del proyecto, **úsalo**; si falla, reintenta 1 vez antes de notificar al usuario y proponer alternativas.

Peticiones de cambios (plantilla)
Cuando pidas una modificación, incluye exactamente:
1. Objetivo claro (1-2 frases).
2. Archivos afectados por ruta (p.ej. `src/components/Hero/Hero.astro`).
3. Fragmento de código o líneas relevantes.
4. Comportamiento esperado y criterios de aceptación.
5. Comandos/local testing que quieres que use (opcional).

Parcheo y commits
- Usa `apply_patch` para editar archivos.
- Si un cambio afecta a más de 3 archivos, sugiere dividirlo en PRs pequeños.

Buenas prácticas
- Prefiere cambios locales y puntuales; no reescribir archivos no relacionados.
- Para imágenes, prioriza WebP/AVIF y `srcset`.

Contacto
- Si necesitas acceso a assets privados (imagenes fuente, credenciales), pide instrucciones explícitas al maintainer.

# Copilot Instructions — mcp-context-cache

This MCP server provides intelligent context caching tools for AI agents working with large codebases.

## PROHIBITED — do not use these tools to read project files

**NEVER call `read_file`, `list_dir`, `file_search`, `semantic_search`, or `grep_search` to read project source files.**
These built-in tools are prohibited when `mcp-context-cache` is available.
Only fall back to them if all MCP tools return an error.

## MANDATORY first step

This project has a `contextcache.json`. **Call `get_context_from_config` before any other tool:**

```json
{ "projectRoot": "<absolute-path-to-this-repo>" }
```

For module-level exploration use `get_directory_context`.
For specific files use `get_project_context` with a `paths` array.

## Project Overview

**mcp-context-cache** is a Model Context Protocol (MCP) server. Agents can use its three tools to load project context efficiently:

- `get_project_context` — Load specific files by path list
- `get_directory_context` — Load all files under a directory
- `get_context_from_config` — Load curated context from `contextcache.json`

Versión: 2026-05-14
