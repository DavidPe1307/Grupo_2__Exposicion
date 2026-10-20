# Trazabilidad · Tarea 1 · Registrar evaluación

**Pregunta que responde:** ¿algún requisito se perdió en el camino de la idea al wireframe?

Se lee por filas: se empieza en el requisito y se sigue hasta el cuadro del wireframe donde se puede ver y probar.

## Matriz requisito → artefactos
| Requisito | Sitemap (`02`) | Navegación (`03`) | User flow (`04`) | Componentes (`05`) | Wireframe Lo-Fi (`06`) |
|---|---|---|---|---|---|
| **R1** Llegar al formulario desde el dashboard | 1.0 Dashboard → 2.0 Registrar prueba | Nav. #1: menú lateral o «+ Nueva evaluación» | Pasos 1 y 2 | Menú lateral · Botón «+ Nueva evaluación» | Cuadro 1 |
| **R2** Escribir quién fue evaluado y qué tarea hizo | 2.0 Registrar prueba | (ya está en la pantalla) | Paso 3 · Llenar campos | Formulario de registro · Campo de texto | Cuadro 2 |
| **R3** Escribir tiempo, errores, resultado y satisfacción | 2.0 Registrar prueba | (ya está en la pantalla) | Paso 3 · Llenar campos | Campo de texto · Lista desplegable · Selector 1–5 | Cuadro 2 |
| **R4** Escribir sus observaciones | 2.0 Registrar prueba | (ya está en la pantalla) | Paso 3 · Llenar campos | Campo de texto (área) | Cuadro 2 |
| **R5** Enterarse si dejó un dato obligatorio vacío o mal | 2.0 Registrar prueba | Nav. #2: se queda y corrige (error bajo el campo; Guardar deshabilitado) | Paso 4 · rama «No» | Mensaje de error · Botón «Guardar» (deshabilitado) | Cuadro 3 (marcas A y B) |
| **R6** Guardar y ver que quedó guardado | 1.0 Dashboard (resultado) | Nav. #3: Guardar → Dashboard | Pasos 5 y 6 | Botón «Guardar» · Mensaje de éxito · Tarjeta de conteo | Cuadro 4 (marcas A y B) |

## Elementos que no son requisito, y por qué existen
| Elemento | Dónde está | Justificación |
|---|---|---|
| Botón «Cancelar» | Nav. #4 · Cuadros 2 y 3 | Salida del usuario (H3). No es un requisito aparte. |
| Menú lateral con ítem activo | Nav. #5 · todos los cuadros | Consistencia y ubicación (H1, H4). Es parte de R1. |
| Filtros, tabla de hallazgos, barras de problemas frecuentes | Cuadros 1 y 4 | Contexto del Dashboard general del proyecto (HU-02). Ver `05-componentes.md`. |
| Banner de escala de severidad | Cuadros 2 y 3 | Ayuda al evaluador para no depender de su memoria. Ver `docs/decisiones.md`. |

## Cobertura por cuadro de wireframe
| Cuadro | Momento del user flow | Archivo Lo-Fi | Requisitos |
|---|---|---|---|
| 1 | Dashboard (pasos 1–2) | `06-wireframes/lofi/wireframes_tarea1_lofi01.png` (cuadro 1) | R1 |
| 2 | Formulario vacío (paso 3) | idem (cuadro 2) | R2, R3, R4 |
| 3 | Formulario con error (paso 4, rama «No») | idem (cuadro 3) | R5 |
| 4 | Dashboard tras guardar (pasos 5–6) | idem (cuadro 4) | R6 |

Las versiones Mid-Fi (`midfi/`) y Hi-Fi (`hifi/`) repiten los mismos 4 cuadros con más detalle: son un adelanto de la Fase 2.

## Comprobación (prueba de fuego)
- [x] Ninguna celda de la matriz está vacía: todo requisito tiene pantalla, navegación, flujo, componentes y cuadro.
- [x] Todo cuadro del wireframe corresponde a al menos un requisito (nada sobra).
- [x] Todo nodo del user flow tiene su cuadro (Dashboard, Registrar prueba, Llenar campos, ¿Datos válidos?/Error, Guardar, Dashboard + éxito).
- [x] Todo componente del inventario aparece dibujado en algún cuadro.
- [x] Los nombres son iguales en el sitemap, el menú y los títulos de las pantallas.
