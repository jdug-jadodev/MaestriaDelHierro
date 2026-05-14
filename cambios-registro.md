# 📊 Registro de Cambios con Estadísticas
**Iniciado:** 14/5/2026, 3:36:37 p. m.
**Proyecto:** C:\Users\Usuario\Documents\Maestria-del-hierro\MaestriaDelHierro
**Formato:** Archivos nuevos, modificados y eliminados
**Estado:** Monitoreando cambios no commiteados


## 🕐 14/05/2026, 15:36:38

### 📊 Resumen
- **Total archivos:** 8
- **📝 Nuevos:** 8
- **✏️ Modificados:** 0
- **🗑️ Eliminados:** 0
- **Líneas añadidas:** +0
- **Líneas eliminadas:** -0
- **Balance neto:** 0 líneas

### 📝 Detalle por archivo

| Estado | Archivo | Añadidas | Eliminadas | Neto |
|--------|---------|----------|------------|------|
| 🆕 | `copilot-instructions.md` | nuevo | -0 | 0 |
| 🆕 | `monitor.cjs` | nuevo | -0 | 0 |
| 🆕 | `project.INSTRUCTIONS.md` | nuevo | -0 | 0 |
| 🆕 | `public/INSTRUCTIONS.md` | nuevo | -0 | 0 |
| 🆕 | `src/components/INSTRUCTIONS.md` | nuevo | -0 | 0 |
| 🆕 | `src/layouts/INSTRUCTIONS.md` | nuevo | -0 | 0 |
| 🆕 | `src/pages/INSTRUCTIONS.md` | nuevo | -0 | 0 |
| 🆕 | `src/styles/INSTRUCTIONS.md` | nuevo | -0 | 0 |

### 📁 Lista completa

<details>
<summary>Ver todos los archivos (8)</summary>

**🆕 Nuevos:**
```
copilot-instructions.md
monitor.cjs
project.INSTRUCTIONS.md
public/INSTRUCTIONS.md
src/components/INSTRUCTIONS.md
src/layouts/INSTRUCTIONS.md
src/pages/INSTRUCTIONS.md
src/styles/INSTRUCTIONS.md
```

</details>

---

## 🕐 14/05/2026, 15:36:51

### 📊 Resumen
- **Total archivos:** 8
- **📝 Nuevos:** 0
- **✏️ Modificados:** 8
- **🗑️ Eliminados:** 0
- **✅ En staging:** 8 (listos para commit)
- **Líneas añadidas:** +574
- **Líneas eliminadas:** -0
- **Balance neto:** +574 líneas

### 📝 Detalle por archivo

| Estado | Archivo | Añadidas | Eliminadas | Neto |
|--------|---------|----------|------------|------|
| ✅ ✏️ | `monitor.cjs` | +430 | -0 | +430 |
| ✅ ✏️ | `copilot-instructions.md` | +53 | -0 | +53 |
| ✅ ✏️ | `src/components/INSTRUCTIONS.md` | +23 | -0 | +23 |
| ✅ ✏️ | `project.INSTRUCTIONS.md` | +16 | -0 | +16 |
| ✅ ✏️ | `src/pages/INSTRUCTIONS.md` | +15 | -0 | +15 |
| ✅ ✏️ | `src/layouts/INSTRUCTIONS.md` | +14 | -0 | +14 |
| ✅ ✏️ | `src/styles/INSTRUCTIONS.md` | +13 | -0 | +13 |
| ✅ ✏️ | `public/INSTRUCTIONS.md` | +10 | -0 | +10 |

### 📁 Lista completa

<details>
<summary>Ver todos los archivos (8)</summary>

**✅ Modificados (staged):**
```
monitor.cjs
copilot-instructions.md
src/components/INSTRUCTIONS.md
project.INSTRUCTIONS.md
src/pages/INSTRUCTIONS.md
src/layouts/INSTRUCTIONS.md
src/styles/INSTRUCTIONS.md
public/INSTRUCTIONS.md
```

</details>

### 💻 Código Añadido

**copilot-instructions.md** (+53 líneas)**

```
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
```

**monitor.cjs** (+430 líneas)**

```
const { exec } = require('child_process');
const fs = require('fs');
const path = require('path');

const OUTPUT_FILE = 'cambios-registro.md';
const PROJECT_PATH = process.cwd();
let lastChanges = '';
let lastCommitHash = '';
let debounceTimer = null;
let commitCheckTimer = null;

// Inicializar archivo
fs.writeFileSync(OUTPUT_FILE, `# 📊 Registro de Cambios con Estadísticas
**Iniciado:** ${new Date().toLocaleString()}
**Proyecto:** ${PROJECT_PATH}
**Formato:** Archivos nuevos, modificados y eliminados
**Estado:** Monitoreando cambios no commiteados

`);

console.log('🔍 Monitoreando proyecto (incluye archivos nuevos)...');
console.log(`📝 Registro: ${OUTPUT_FILE}`);
console.log('🛑 Ctrl+C para detener\n');
console.log('📌 El registro se limpiará automáticamente después de cada commit\n');

// Función para obtener el último commit hash
function getLastCommitHash(callback) {
 exec('git rev-parse HEAD', (err, stdout) => {
 if (err) {
 callback('');
 return;
 }
 callback(stdout.trim());
 });
}

// Función para verificar si hubo un nuevo commit
function checkForNewCommit() {
 getLastCommitHash((currentHash) => {
 if (currentHash && currentHash !== lastCommitHash) {
 if (lastCommitHash !== '') {
 console.log('\n📦 Nuevo commit detectado! Borrando archivo de registro...\n');

// Obtener información del último commit
 exec('git log -1 --pretty=format:"%h - %s (%cr)"', (err, commitInfo) => {
 const commitMessage = err ? 'Commit realizado' : commitInfo;

// BORRAR el archivo completamente
 try {
 fs.unlinkSync(OUTPUT_FILE);
 console.log(`✅ Archivo ${OUTPUT_FILE} eliminado`);
 } catch (error) {
 console.log(`⚠️ No se pudo eliminar el archivo: ${error.message}`);
 }

// Crear un NUEVO archivo con el mensaje del commit
 const newHeader = `# 📊 Registro de Cambios con Estadísticas
**Iniciado:** ${new Date().toLocaleString()}
**Proyecto:** ${PROJECT_PATH}
**Último commit:** ${commitMessage}
**Estado:** Monitoreando nuevos cambios

`;

 fs.writeFileSync(OUTPUT_FILE, newHeader);

// Reiniciar el registro para nuevos cambios
 lastChanges = '';

// Mostrar confirmación
 console.log(`✅ Nuevo archivo creado con información del commit: ${commitMessage}`);
 console.log('📝 Registro reiniciado para nuevos cambios\n');
 });
 }
 lastCommitHash = currentHash;
 }
 });
}

// Función para obtener archivos nuevos (untracked)
function getUntrackedFiles(callback) {
 exec('git ls-files --others --exclude-standard', (err, stdout) => {
 if (err) {
 callback([]);
 return;
 }

 const files = stdout.split('\n')
 .filter(f => f.trim() && !f.includes('cambios-registro.md'))
 .filter((f, i, self) => self.indexOf(f) === i);

 callback(files);
 });
}

// Función para obtener estadísticas detalladas de cambios
function getGitStats(callback) {
 exec('git diff --numstat && git diff --staged --numstat',
 { maxBuffer: 1024 * 1024 },
 (err, stdout) => {
 if (err) {
 callback([]);
 return;
 }

 const files = [];
 const lines = stdout.split('\n').filter(line => line.trim());

 lines.forEach(line => {
 const parts = line.split('\t');
 if (parts.length >= 3) {
 const added = parts[0] === '-' ? 0 : parseInt(parts[0]) || 0;
 const deleted = parts[1] === '-' ? 0 : parseInt(parts[1]) || 0;
 const filename = parts[2];

 if (filename && !filename.includes('cambios-registro.md')) {
 files.push({
 nombre: filename,
 añadidas: added,
 eliminadas: deleted,
 estado: 'modificado',
 extension: path.extname(filename)
 });
 }
 }
 });

 callback(files);
 });
}

// Función para obtener las líneas de código añadidas en cada archivo
function getAddedLines(callback) {
 exec('git diff && git diff --staged',
 { maxBuffer: 1024 * 1024 * 5 },
 (err, stdout) => {
 if (err) {
 callback({});
 return;
 }

 const fileChanges = {};
 const diffLines = stdout.split('\n');
 let currentFile = null;

 diffLines.forEach(line => {
 // Detectar el archivo actual
 if (line.startsWith('diff --git')) {
 const match = line.match(/b\/(.+)$/);
 if (match) {
 currentFile = match[1];
 if (!currentFile.includes('cambios-registro.md')) {
 fileChanges[currentFile] = [];
 }
 }
 } else if (currentFile && !currentFile.includes('cambios-registro.md')) {
 // Capturar líneas añadidas (comienzan con + pero no +++)
 if (line.startsWith('+') && !line.startsWith('+++')) {
 fileChanges[currentFile].push(line.substring(1)); // Quitar el +
 }
 }
 });

 callback(fileChanges);
 });
}

// Función para obtener archivos eliminados
function getDeletedFiles(callback) {
 exec('git ls-files --deleted', (err, stdout) => {
 if (err) {
 callback([]);
 return;
 }

 const files = stdout.split('\n')
 .filter(f => f.trim() && !f.includes('cambios-registro.md'));

 callback(files);
 });
}

// Función para obtener archivos en staging
function getStagedFiles(callback) {
 exec('git diff --staged --name-only', (err, stdout) => {
 if (err) {
 callback([]);
 return;
 }

 const files = stdout.split('\n')
 .filter(f => f.trim() && !f.includes('cambios-registro.md'));

 callback(files);
 });
}

function checkAllChanges() {
 Promise.all([
 new Promise(resolve => getGitStats(resolve)),
 new Promise(resolve => getUntrackedFiles(resolve)),
 new Promise(resolve => getDeletedFiles(resolve)),
 new Promise(resolve => getStagedFiles(resolve)),
 new Promise(resolve => getAddedLines(resolve))
 ]).then(([modifiedFiles, untrackedFiles, deletedFiles, stagedFiles, addedLines]) => {

// Convertir archivos
 const newFiles = untrackedFiles.map(f => ({
 nombre: f,
 añadidas: 0,
 eliminadas: 0,
 estado: 'nuevo',
 extension: path.extname(f)
 }));

 const deletedFilesFormatted = deletedFiles.map(f => ({
 nombre: f,
 añadidas: 0,
 eliminadas: 0,
 estado: 'eliminado',
 extension: path.extname(f)
 }));

// Marcar archivos en staging
 const stagedSet = new Set(stagedFiles);
 const allFiles = [...modifiedFiles, ...newFiles, ...deletedFilesFormatted].map(f => {
 if (stagedSet.has(f.nombre)) {
 return { ...f, estado: f.estado === 'nuevo' ? 'nuevo (staged)' : 'modificado (staged)' };
 }
 return f;
 });

 if (allFiles.length === 0) return;

// Crear identificador único
 const changesId = allFiles.map(f =>
 `${f.nombre}:${f.estado}:${f.añadidas}:${f.eliminadas}`
 ).join('|');

 if (changesId !== lastChanges) {
 const timestamp = new Date().toLocaleString('es-CO', {
 hour12: false,
 year: 'numeric',
 month: '2-digit',
 day: '2-digit',
 hour: '2-digit',
 minute: '2-digit',
 second: '2-digit'
 });

// Calcular estadísticas
 const totalAñadidas = allFiles.reduce((sum, f) => sum + f.añadidas, 0);
 const totalEliminadas = allFiles.reduce((sum, f) => sum + f.eliminadas, 0);
 const totalNeto = totalAñadidas - totalEliminadas;

 const nuevos = allFiles.filter(f => f.estado.includes('nuevo')).length;
 const modificados = allFiles.filter(f => f.estado.includes('modificado')).length;
 const eliminados = allFiles.filter(f => f.estado === 'eliminado').length;
 const staged = allFiles.filter(f => f.estado.includes('staged')).length;

// Crear entrada en Markdown
 let logEntry = `\n## 🕐 ${timestamp}\n\n`;
 logEntry += `### 📊 Resumen\n`;
 logEntry += `- **Total archivos:** ${allFiles.length}\n`;
 logEntry += `- **📝 Nuevos:** ${nuevos}\n`;
 logEntry += `- **✏️ Modificados:** ${modificados}\n`;
 logEntry += `- **🗑️ Eliminados:** ${eliminados}\n`;
 if (staged > 0) {
 logEntry += `- **✅ En staging:** ${staged} (listos para commit)\n`;
 }
 logEntry += `- **Líneas añadidas:** +${totalAñadidas}\n`;
 logEntry += `- **Líneas eliminadas:** -${totalEliminadas}\n`;
 logEntry += `- **Balance neto:** ${totalNeto > 0 ? '+' : ''}${totalNeto} líneas\n\n`;

 logEntry += `### 📝 Detalle por archivo\n\n`;
 logEntry += `| Estado | Archivo | Añadidas | Eliminadas | Neto |\n`;
 logEntry += `|--------|---------|----------|------------|------|\n`;

 allFiles.sort((a, b) => {
 const estadoOrder = {
 'nuevo (staged)': 0,
 'nuevo': 1,
 'modificado (staged)': 2,
 'modificado': 3,
 'eliminado': 4
 };
 return (estadoOrder[a.estado] || 99) - (estadoOrder[b.estado] || 99) ||
 (b.añadidas + b.eliminadas) - (a.añadidas + a.eliminadas);
 });

 allFiles.forEach(f => {
 const neto = f.añadidas - f.eliminadas;
 const netoStr = neto > 0 ? `+${neto}` : neto.toString();

// Emoji según estado
 let estadoEmoji = '✏️';
 if (f.estado.includes('nuevo')) estadoEmoji = '🆕';
 if (f.estado.includes('eliminado')) estadoEmoji = '🗑️';
 if (f.estado.includes('staged')) estadoEmoji = '✅ ' + estadoEmoji;

// Truncar nombre
 let nombreDisplay = f.nombre;
 if (nombreDisplay.length > 50) {
 const parts = nombreDisplay.split(path.sep);
 if (parts.length > 3) {
 nombreDisplay = `.../${parts.slice(-3).join('/')}`;
 }
 }

 const añadidasDisplay = f.estado.includes('nuevo') ? 'nuevo' : `+${f.añadidas}`;
 const eliminadasDisplay = f.estado === 'eliminado' ? 'eliminado' : `-${f.eliminadas}`;

 logEntry += `| ${estadoEmoji} | \`${nombreDisplay}\` | ${añadidasDisplay} | ${eliminadasDisplay} | ${netoStr} |\n`;
 });

 logEntry += `\n### 📁 Lista completa\n\n`;
 logEntry += `<details>\n`;
 logEntry += `<summary>Ver todos los archivos (${allFiles.length})</summary>\n\n`;

// Separar por tipo
 const tipos = {
 '🆕 Nuevos (staged)': allFiles.filter(f => f.estado === 'nuevo (staged)'),
 '🆕 Nuevos': allFiles.filter(f => f.estado === 'nuevo'),
 '✅ Modificados (staged)': allFiles.filter(f => f.estado === 'modificado (staged)'),
 '✏️ Modificados': allFiles.filter(f => f.estado === 'modificado'),
 '🗑️ Eliminados': allFiles.filter(f => f.estado === 'eliminado')
 };

 for (const [titulo, archivos] of Object.entries(tipos)) {
 if (archivos.length > 0) {
 logEntry += `**${titulo}:**\n\`\`\`\n`;
 archivos.forEach(f => {
 logEntry += `${f.nombre}\n`;
 });
 logEntry += '```\n\n';
 }
 }

 logEntry += `</details>\n\n`;

// Mostrar líneas de código añadidas
 const filesWithAddedLines = Object.keys(addedLines).filter(f => addedLines[f].length > 0);
 if (filesWithAddedLines.length > 0) {
 logEntry += `### 💻 Código Añadido\n\n`;
 filesWithAddedLines.forEach(filename => {
 const lines = addedLines[filename];
 if (lines.length > 0) {
 logEntry += `**${filename}** (+${lines.length} línea${lines.length > 1 ? 's' : ''})**\n\n`;
 logEntry += '```\n';
 lines.forEach(line => {
 logEntry += `${line}\n`;
 });
 logEntry += '```\n\n';
 }
 });
 }

 logEntry += `---\n`;

// Guardar en archivo
 fs.appendFileSync(OUTPUT_FILE, logEntry);

// Mostrar en consola
 console.log(`\n🕐 ${timestamp}`);
 console.log(`📊 Total: ${allFiles.length} archivos (🆕 ${nuevos}, ✏️ ${modificados}, 🗑️ ${eliminados})`);
 if (staged > 0) {
 console.log(` ✅ ${staged} archivos en staging (listos para commit)`);
 }
 console.log(` Líneas: +${totalAñadidas} / -${totalEliminadas} (${totalNeto > 0 ? '+' : ''}${totalNeto})`);

 lastChanges = changesId;
 }
 });
}

// Usar debounce
function debouncedCheck() {
 if (debounceTimer) clearTimeout(debounceTimer);
 debounceTimer = setTimeout(checkAllChanges, 500);
}

// Inicializar último commit hash
getLastCommitHash((hash) => {
 lastCommitHash = hash;
 console.log(`📌 Último commit: ${hash ? hash.substring(0, 7) : 'Ninguno'}`);
});

// Verificar commits cada 2 segundos
commitCheckTimer = setInterval(checkForNewCommit, 2000);

// Monitorear cambios en el sistema de archivos
try {
 const ignoredDirs = ['node_modules', '.git', 'target', 'build', 'dist', 'packages.json', 'package-lock.json', 'yarn.lock', 'pnpm-lock.yaml'];

 const watcher = fs.watch(PROJECT_PATH, { recursive: true }, (eventType, filename) => {
 if (!filename) return;

 const shouldIgnore = ignoredDirs.some(dir =>
 filename.includes(dir) || filename.includes('\\' + dir + '\\')
 );

 if (!shouldIgnore && !filename.includes(OUTPUT_FILE)) {
 debouncedCheck();
 }
 });

 console.log('⚡ Modo tiempo real con detección de archivos nuevos activado');
 console.log('📦 Detectando commits automáticamente...\n');

// Check inicial
 setTimeout(checkAllChanges, 1000);

// Backup cada 2 segundos
 setInterval(checkAllChanges, 2000);

} catch (err) {
 console.log('⚠️ Usando modo intervalo');
 setInterval(checkAllChanges, 1000);
}

// Manejar cierre
process.on('SIGINT', () => {
 console.log('\n\n👋 Monitoreo detenido');
 console.log(`📝 Registro guardado en: ${OUTPUT_FILE}`);

 if (commitCheckTimer) clearInterval(commitCheckTimer);

 fs.appendFileSync(OUTPUT_FILE, `\n*Monitor detenido: ${new Date().toLocaleString()}*\n`);
 process.exit();
});
```

**project.INSTRUCTIONS.md** (+16 líneas)**

```
# INSTRUCTIONS — Resumen de proyecto

Descripción
- Sitio corporativo construido con Astro y Tailwind; estructura simple y enfocada en contenido estático.

Archivos de interés
- `package.json` — dependencias y scripts.
- `astro.config.mjs`, `tailwind.config.mjs`, `tsconfig.json` — configuración del proyecto.
- `monitor.cjs` — script del repositorio (abrir para ver propósito específico).

Decisiones y notas de diseño
- Usar componentes pequeños y reutilizables.
- Evitar lógica de servidor compleja dentro de las páginas; optar por pre-rendering de Astro.

Contacto
- Si hay dudas sobre convenciones, mencionar la sección correspondiente en `copilot-instructions.md`.
```

**public/INSTRUCTIONS.md** (+10 líneas)**

```
# INSTRUCTIONS — public

Propósito
- Recursos estáticos: imágenes, assets y archivos públicos como `robots.txt`.

Convenciones
- Mantener assets optimizados (WebP/AVIF para web). Rutas relativas desde los componentes.

Al editar
- Si reemplazas imágenes, conserva nombres o actualiza referencias en componentes/páginas.
```

**src/components/INSTRUCTIONS.md** (+23 líneas)**

```
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
```

**src/layouts/INSTRUCTIONS.md** (+14 líneas)**

```
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
```

**src/pages/INSTRUCTIONS.md** (+15 líneas)**

```
# INSTRUCTIONS — src/pages

Propósito
- Contiene las páginas del sitio: `index.astro`, `home.astro`, `portfolio.astro`.

Responsabilidades
- Páginas: ensamblan componentes, definen contenido y datos estáticos.
- Evitar lógica compleja en las páginas; si necesitas datos dinámicos, plantéalo como un servicio o helper.

Rutas importantes
- `/` y `/home` — página principal.
- `/portfolio` — galería/portfolio.

Al pedir cambios en una página
- Indica la URL objetivo y el componente afectado. Si el cambio es de contenido, proporciona el texto final.
```

**src/styles/INSTRUCTIONS.md** (+13 líneas)**

```
# INSTRUCTIONS — src/styles

Propósito
- Ubicar estilos globales y variables CSS.

Archivo clave
- `global.css` — estilos globales y reset; preferir utilidades de Tailwind para estilos comunes.

Convenciones
- Evitar duplicar reglas en componentes; usa clases utilitarias de Tailwind cuando sea posible.

Al editar
- Si añades variables o utilidades, documenta su uso y añade ejemplos de clase.
```

---
