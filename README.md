# 100hires-portfolio

Portfolio del proceso de selección laboral 100hires — Franco Giglio

---

## Herramientas instaladas

### Cursor IDE
Editor de código basado en VS Code con capacidades de IA integradas. Disponible en [cursor.com](https://www.cursor.com/).

### Claude Code for VS Code (Anthropic)
Extensión oficial de Anthropic para VS Code / Cursor que integra el asistente Claude directamente en el editor. Permite hacer preguntas, generar código y navegar el codebase usando lenguaje natural.

### Codex (OpenAI)
Extensión de OpenAI para VS Code / Cursor que provee sugerencias de código y autocompletado basado en el modelo Codex.

---

## Pasos completados

1. **Descarga e instalación de Cursor IDE** — Descargué el instalador desde cursor.com y lo instalé en Windows.
2. **Instalación de extensión "Claude Code for VS Code"** — Busqué "Claude Code" en el Marketplace de Cursor y lo instalé desde el editor.
3. **Instalación de extensión "Codex"** — Busqué "Codex" de OpenAI en el Marketplace de Cursor y lo instalé desde el editor.
4. **Creación de la carpeta local `100hires-portfolio`** — Creé la carpeta en el sistema local y la abrí en Cursor (File > Open Folder).
5. **Creación de este archivo `README.md`** — Documenté el proceso completo.
6. **Publicación en GitHub** — Creé el repositorio público `100hires-portfolio` en la cuenta `francogiglio1801` y subí el archivo.

---

## Problemas encontrados y soluciones

### 1. El Marketplace de Cursor no siempre muestra extensiones del VS Code Marketplace oficial
- **Problema:** Algunas extensiones disponibles en el VS Code Marketplace no aparecen en la búsqueda de Cursor por defecto, ya que Cursor usa su propio registry (Open VSX).
- **Solución:** Se puede habilitar el acceso al marketplace de VS Code desde la configuración de Cursor, o buscar el ID exacto de la extensión e instalarla manualmente.

### 2. Configuración de git para el primer push
- **Problema:** Al inicializar el repo localmente, git requería configurar usuario y email antes de hacer el primer commit.
- **Solución:** Se ejecutaron los comandos `git config --global user.name` y `git config --global user.email` con los datos de la cuenta de GitHub.

### 3. Autenticación con GitHub desde la terminal
- **Problema:** Al intentar hacer `git push`, GitHub solicitó autenticación. Las contraseñas tradicionales ya no son aceptadas por HTTPS.
- **Solución:** Se generó un Personal Access Token (PAT) desde GitHub Settings > Developer settings y se usó ese token como contraseña.

---

## Repositorio

- **GitHub:** [https://github.com/francogiglio1801/100hires-portfolio](https://github.com/francogiglio1801/100hires-portfolio)
- **Autor:** Franco Giglio (@francogiglio1801)
- **Fecha:** Junio 2026
