# HCI-2026-G2 · Prototipos y wireframes: de requisitos a arquitectura, flujo y wireframe

Universidad Técnica de Ambato · FISEI · Software · 5.º semestre, paralelo B
Interacción Humano-Computador · APE 4, Fase 1 · Grupo 2

<!-- [SHEYLA] -->
## 1. Problema

Al diseñar una aplicación es habitual pasar de los requisitos directamente a dibujar o programar pantallas, sin un proceso intermedio. Cuando eso ocurre aparecen interfaces inconsistentes, flujos incompletos, componentes que nadie pidió y requisitos que nunca llegan a verse en el diseño. Corregirlo después, cuando ya existe código, es costoso.

Este trabajo aborda cómo pasar de los requisitos a la arquitectura, el flujo y el wireframe de forma ordenada y verificable, de modo que cada requisito pueda seguirse hasta una pantalla.

## 2. Objeto de estudio y objetivos

**Objeto de estudio:** el proceso de definir sitemap, navegación, user flow, componentes y wireframes de baja fidelidad, aplicado a la Tarea 1 «Registrar evaluación» del proyecto Usability Test Dashboard 2.0. La tarea se usa como ejemplo didáctico; el proyecto completo está en `resultados/proyecto-real/`.

**Objetivo general:** enseñar a la clase, con un caso simple y reproducible, cómo se pasa de requisitos a wireframes y cómo se comprueba que ningún requisito se pierde en el camino.

**Objetivos específicos:**
- Redactar los requisitos R1–R6 de la tarea a partir de las historias de usuario.
- Construir el sitemap, la navegación, el user flow, el inventario de componentes y los wireframes Lo-Fi.
- Verificar con una matriz de trazabilidad que cada requisito llega hasta un wireframe.
- Dejar una plantilla en blanco para que la clase repita el ejercicio con su propio caso.

## 5. Herramientas

| Herramienta | Uso |
|---|---|
| Figma / Penpot | Diagramas y wireframes (Lo-Fi, y Mid-Fi y Hi-Fi como adelanto de la siguiente fase) |
| GitHub | Repositorio, issues, ramas y Pull Requests con revisión cruzada |
| Markdown | Documentación (requisitos, navegación, componentes, trazabilidad) |
| Gemini (NotebookLM) | Generación de las diapositivas de la exposición |
| Kahoot | Evaluación de lo aprendido en clase |
| Asistentes de IA (Claude, Gemini) | Apoyo en la organización del contenido y la revisión; el equipo revisó y ajustó los resultados |
<!-- [/SHEYLA] -->

<!-- [MARTIN] -->
## 3. Conceptos HCI
- **Requisitos:** lo que el usuario necesita poder hacer con el sistema. Se redactan desde su punto de vista, con un solo verbo, y se numeran (R1, R2…) para poder seguirlos hasta el wireframe. Responden: ¿qué debe poder hacer el sistema?
- **Sitemap:** árbol que muestra qué pantallas existen y de cuál cuelga cada una. Responde: ¿qué pantallas existen? Lleva leyenda y cada requisito debe ocurrir en alguna pantalla. No lleva flechas de recorrido, eso es del user flow.
- **Navegación:** los elementos visibles (menús, botones, enlaces) que permiten pasar de una pantalla a otra. Debe ser consistente, mostrar dónde está el usuario, ofrecer siempre una salida y definir adónde regresa tras guardar o cancelar.
- **Heurísticas de Nielsen aplicadas:** H1 visibilidad del estado, H3 control y libertad, H4 consistencia y H5 prevención de errores.

## 4. Procedimiento
1. Se partió de la historia de Ana, la evaluadora, y se escribieron los requisitos R1–R6 con un verbo cada uno (`prototipos/01-requisitos.md`).
2. Se dibujó el sitemap con simbología y leyenda, ubicando cada requisito en una pantalla (`prototipos/02-sitemap.png`).
3. Se armó la tabla de navegación (de dónde → a dónde → con qué elemento) y el mapa, definiendo adónde regresa el usuario tras Guardar y Cancelar (`prototipos/03-navegacion.md` y `.png`).
4. Se registraron las versiones en la bitácora (`evidencias/bitacora-martin.md`).
5. Cada entrega se subió con commits pequeños y Pull Request revisado por un compañero.
<!-- [/MARTIN] -->

<!-- [DAVID] -->
## 6. Resultados
| Producto | Ubicación |
|---|---|
| Requisitos | `prototipos/01-requisitos.md` |
| Sitemap, navegación, user flow, componentes | `prototipos/02` a `05` |
| Wireframes Lo-Fi (y adelanto Mid-Fi / Hi-Fi) | `prototipos/06-wireframes/` |
| Trazabilidad | `prototipos/07-trazabilidad.md` |
| Plantilla para repetir el ejercicio | `prototipos/plantilla-en-blanco.md` |
| Decisiones de diseño | `docs/decisiones.md` |
| Investigación completa | `docs/investigacion.md` |
| Borradores y capturas | `evidencias/` |
| Presentación y resultado del Kahoot | `resultados/` |

## 7. Integrantes
| Integrante | Aporte principal |
|---|---|
| Martín Palacios | Requisitos, sitemap y navegación |
| David Pérez | User flow, componentes y administración del repositorio |
| Sheyla Pacha | Wireframes, fidelidad y trazabilidad |

Detalle en `CONTRIBUCIONES.md`.
<!-- [/DAVID] -->

## 8. Conclusiones
Ver `docs/conclusiones.md`.

## 9. Cómo reproducir el ejercicio
Usa `prototipos/plantilla-en-blanco.md` y sigue los 7 pasos con un caso propio.
