# Plataforma de Estructuras de Datos Avanzadas

Sitio educativo del curso CS3014 construido con Astro. Presenta teoría, operaciones, ejemplos, ejercicios y visualizaciones de estructuras de datos avanzadas. El contenido del curso se organiza a partir de [`content/knowledge-map.json`](content/knowledge-map.json), que enlaza cada tema con el material fuente de `raw-materials/`.

## Requisitos

- Node.js 22.12 o superior (según `package.json`)
- pnpm

## Instalación y uso

```bash
git clone https://github.com/Auky216/EDA-Platform.git
cd EDA-Platform
pnpm install --frozen-lockfile
pnpm dev
```

Astro mostrará la dirección local del servidor. Para generar y revisar la versión de producción:

```bash
pnpm check
pnpm test
pnpm build
pnpm preview
```

`pnpm check` comprueba la coherencia entre el mapa de conocimiento y los archivos del curso. `pnpm build` valida el contenido contra los esquemas del proyecto.

## Organización

- `content/knowledge-map.json`: índice y fuente de verdad de los temas.
- `content/structures/`: teoría, operaciones, ejemplos y ejercicios.
- `cpp/structures/`: implementaciones y pasos en C++.
- `raw-materials/`: materiales fuente del curso.
- `src/`: páginas, componentes y visualizaciones.
- `scripts/`: verificaciones y tareas de mantenimiento.

## Contribuir

Lee [AGENTS.md](AGENTS.md) y [CONTENT-AGENT-RULES.md](CONTENT-AGENT-RULES.md) antes de modificar contenido. No agregues temas que no estén respaldados por el mapa de conocimiento y el material fuente. En un PR, indica la semana o estructura afectada y ejecuta `pnpm check`, `pnpm test` y `pnpm build`.

## Estado y licencia

Proyecto académico en desarrollo. Los materiales de `raw-materials/` pueden tener derechos de terceros. No se declara una licencia de reutilización para el conjunto del repositorio; consulta a sus titulares antes de redistribuirlo.
