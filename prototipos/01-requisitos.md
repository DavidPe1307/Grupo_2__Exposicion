# Requisitos de la Tarea 1 · Registrar evaluación

**Proyecto:** Usability Test Dashboard 2.0 · **Actor:** Ana, evaluadora de usabilidad

**Historia:** Ana pone a un participante a usar una aplicación y anota cuánto tardó, cuántos errores
cometió, si logró la tarea y qué tan satisfecho quedó. Después entra al sistema para guardar esos datos.

## Regla
Un requisito, un verbo. Se redacta desde el punto de vista del usuario y se numera (R1, R2…) para
poder seguirlo hasta el wireframe.

## Requisitos
| ID | Ana debe poder... | Verbo | Historia de usuario |
|---|---|---|---|
| R1 | Llegar al formulario desde el dashboard | Llegar | HU-02, HU-11 |
| R2 | Escribir quién fue evaluado y qué tarea hizo | Escribir | HU-01 |
| R3 | Escribir tiempo, errores, resultado y satisfacción | Escribir | HU-01 |
| R4 | Escribir sus observaciones | Escribir | HU-10 |
| R5 | Enterarse si dejó un dato obligatorio vacío o mal | Enterarse | HU-10 |
| R6 | Guardar y ver que quedó guardado | Guardar | HU-01 |

## Notas
- R2 y R3 agrupan varios campos del mismo bloque del formulario con el mismo verbo. Si se quisiera más
  detalle, se dividirían en requisitos más finos.
- En R6 la acción es guardar; «ver que quedó guardado» es la confirmación de esa misma acción
  (heurística H1, visibilidad del estado).
- **Por qué «Cancelar» no es un requisito aparte:** es la salida del usuario en cualquier momento
  (heurística H3, control y libertad). No es una tarea que Ana quiera lograr, sino una vía de escape
  del formulario; por eso aparece en la navegación y en los componentes, pero no como R7.

## Uso en los demás productos
Estos mismos R1–R6 se usan en el sitemap (pantalla donde ocurre cada uno), el user flow (paso en que
aparece), los componentes (qué pieza lo cubre) y los wireframes (cuadro donde se ve).
