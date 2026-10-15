# Componentes · Tarea 1 · Registrar evaluación

Piezas reutilizables organizadas con Atomic Design (átomo → molécula → organismo).

## Inventario
| Componente | Nivel | Estados que necesita | Requisito | Dónde aparece |
|---|---|---|---|---|
| Menú lateral | Organismo | Normal · ítem activo | R1 | Todas las pantallas |
| Formulario de registro | Organismo | Normal · con error | R2, R3, R4, R5 | Registrar prueba |
| Campo de texto con etiqueta, ayuda y error (incluye variante de área de texto) | Molécula | Normal · foco · error | R2, R4 | Registrar prueba |
| Lista desplegable (Resultado de la tarea) | Molécula | Normal · foco · error | R3 | Registrar prueba |
| Selector 1–5 (Satisfacción) | Molécula | Normal · seleccionado | R3 | Registrar prueba |
| Tarjeta de conteo (Pruebas realizadas) | Molécula | Normal | R6 | Dashboard |
| Botón «+ Nueva evaluación» | Átomo | Normal · foco | R1 | Dashboard |
| Botón «Guardar» | Átomo | Normal · foco · deshabilitado | R5, R6 | Registrar prueba |
| Botón «Cancelar» | Átomo | Normal · foco | Salida del usuario (H3), no es requisito aparte | Registrar prueba |
| Mensaje de error bajo el campo | Átomo | Visible · oculto | R5 | Registrar prueba |
| Mensaje de éxito | Átomo | Visible · oculto | R6 | Dashboard (tras guardar) |

## Elementos de contexto (aparecen en los wireframes, pero no vienen de R1–R6)
Pertenecen al Dashboard general del proyecto (HU-02) y dan contexto a la pantalla; no se crean
componentes nuevos para ellos en esta tarea:
- Filtros (chips) y tabla de hallazgos
- Barras de problemas frecuentes
- Tarjetas «Hallazgos registrados» y «Severidad promedio»
- Banner informativo de escala de severidad en el formulario
- Bloque «Equipo» del menú lateral

## Estados (ejemplo: campo y botón)
| Componente | Normal | Foco | Error / Deshabilitado |
|---|---|---|---|
| Campo de texto | Borde gris | Borde morado grueso | Borde rojo + mensaje «Campo obligatorio» |
| Botón «Guardar» | Morado | Morado con aro de foco | Gris (deshabilitado) |

Los valores exactos de color y borde están en la guía de estilo del proyecto.

## Reglas
1. Si se repite, es componente.
2. Un nombre, una función.
3. Cada componente justifica su existencia con un requisito.
4. Consistencia: la misma pieza se ve y se comporta igual en todas partes.
5. No se crea un componente para algo de uso único sin motivo.
6. Se definen junto con los wireframes.
