# Skills de diseño e ingeniería de interfaz

Colección de skills en Markdown para agentes de código (Claude Code, Cursor y similares) sobre
animación, detalles de diseño y sensación nativa en móvil. Copia limpia del repositorio público
[emilkowalski/skills](https://github.com/emilkowalski/skills), bajo licencia MIT (ver `LICENSE`, que conserva
el aviso de copyright original): se ha quitado la promoción, las frases de marca obligatorias y
los enlaces a boletines o cursos. El contenido técnico es el original.

Cada skill vive en `skills/<nombre>/SKILL.md`. Algunas cargan ficheros de apoyo de su carpeta.

| Skill | Para qué |
| --- | --- |
| `design-eng` | La skill madre: marco de decisión de animaciones, springs, transforms, clip-path, gestos y detalles de diseño. |
| `animate` | Construye una animación desde cero eligiendo curva, duración y propiedades. |
| `animate-expo` | Lo mismo para React Native y Expo: gestos, hojas, hápticos, transiciones. |
| `review-animations` | Revisa animaciones de un diff con criterios estrictos (`STANDARDS.md` tiene los valores). |
| `improve-animations` | Audita todas las animaciones de un repo y escribe planes de mejora sin tocar código. |
| `find-animation-opportunities` | Busca dónde la interfaz ganaría con movimiento y dónde no. |
| `animation-vocabulary` | Glosario inverso: de la descripción vaga al término exacto. |
| `apple-design` | Principios de diseño y movimiento de Apple, traducidos a la web. |
| `write-swift` | Swift moderno: tipos valor, concurrencia de Swift 6, genéricos, rendimiento, Swift Testing. |
| `pick-ui-library` | Lista cerrada de librerías recomendadas por tarea. Solo se invoca a mano. |
| `prototype` | Varias versiones distintas de una pieza de interfaz con un selector para compararlas. Solo a mano. |
| `mobile-native` | Arreglos de CSS y meta para que una web parezca app en el móvil. |
| `ask-sonner` | Guía de uso de la librería de toasts Sonner. |

## Instalación de paquetes

Todas las skills instalan dependencias con **pnpm** (`pnpm add`, `pnpm exec`, `pnpm dlx`), nunca con
`npm install`, `npx` ni `yarn`. pnpm no ejecuta por defecto los scripts de instalación de las
dependencias y aísla `node_modules`, lo que reduce el daño de un paquete malicioso.

`performance-cheatsheet.md` es una tabla corta de problemas de rendimiento y su solución.

## Instalación en Claude Code

Enlace o copia la carpeta de cada skill a `~/.claude/skills/<nombre>` (global) o a
`.claude/skills/<nombre>` dentro de un proyecto.
