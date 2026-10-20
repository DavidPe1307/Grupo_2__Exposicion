# Trazabilidad · Tarea 1 · de requisito a wireframe

Cada requisito se puede seguir de punta a punta. Si una celda queda vacía, falta un artefacto.

| Requisito | Sitemap | Navegación | User flow | Componentes | Wireframe |
|---|---|---|---|---|---|
| **R1** Llegar al formulario desde el dashboard | 1.0 → 2.0 | Menú lateral o «+ Nueva evaluación» | Pasos 1 → 2 | Menú lateral; botón «+ Nueva evaluación» | Cuadro 1 |
| **R2** Escribir identificación (nombre, participante, tarea) | 2.0 Registrar prueba | Ya estás en la pantalla | Paso 3 · Llenar campos | Campo de texto; formulario | Cuadro 2 |
| **R3** Escribir tiempo, errores, resultado y satisfacción | 2.0 Registrar prueba | Ya estás en la pantalla | Paso 3 · Llenar campos | Campo; lista desplegable; selector 1–5 | Cuadro 2 |
| **R4** Escribir observaciones del evaluador | 2.0 Registrar prueba | Ya estás en la pantalla | Paso 3 · Llenar campos | Campo de texto (área) | Cuadro 2 |
| **R5** Saber si un dato obligatorio está vacío o mal | 2.0 Registrar prueba | Error bajo el campo; Guardar deshabilitado | Paso 4 · rama «No» | Mensaje de error; botón Guardar (deshabilitado) | Cuadro 3 |
| **R6** Guardar y ver que quedó guardado | 1.0 Dashboard | Guardar → Dashboard | Pasos 5 → 6 | Botón Guardar; mensaje de éxito; tarjeta de conteo | Cuadro 4 |

> **Nota:** «Cancelar» es la salida del usuario en cualquier momento (heurística H3): aparece en la
> navegación y en los componentes, pero no como requisito aparte.

## Cómo se lee, fila por fila
1. Empieza por el requisito: es lo que el usuario necesita hacer.
2. Sigue la fila: en qué pantalla ocurre (sitemap) y con qué se llega (navegación).
3. Mira en qué paso del user flow aparece y qué piezas lo hacen posible.
4. Termina en el cuadro del wireframe donde se puede ver y probar.
5. Ejemplo R5: error bajo el campo → rama «No» → mensaje de error → cuadro 3.

## Comprobación final
- [ ] Todo requisito tiene pantalla, flujo y wireframe (ninguna celda vacía).
- [ ] Todo wireframe corresponde a algún requisito (nada sobra).
- [ ] Todo componente de la tabla aparece dibujado en un cuadro.
- [ ] Todo nodo del user flow tiene su cuadro de wireframe.
- [ ] Los nombres son iguales en el sitemap, el menú y los títulos.