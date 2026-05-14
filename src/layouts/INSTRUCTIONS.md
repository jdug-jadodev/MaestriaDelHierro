# INSTRUCTIONS — src/layouts

Propósito
- Plantillas y layout globales para envolver las páginas (cabecera, pie y slot de contenido).

Archivo clave
- `Layout.astro` — envoltorio principal usado por las páginas del sitio.

Convenciones
- Layouts deben ser lo más genéricos posible: insertar slots para contenido concreto.
- Evitar lógica pesada o fetches directos en el layout; preferir pasar props desde la página.

Al editar
- Si añades una nueva región (p.ej. barra lateral), documenta en este archivo y actualiza las páginas que lo usan.
