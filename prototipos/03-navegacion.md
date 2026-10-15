# Navegación · Tarea 1 · Registrar evaluación

## Mapa
- **Dashboard → Registrar prueba:** ítem «Registrar prueba» del menú lateral, o botón «+ Nueva evaluación».
- **Registrar prueba → Dashboard:** botón «Guardar» (con datos válidos) o «Cancelar».
- **Registrar prueba → Registrar prueba:** con error, el usuario se queda y corrige.
- **Menú lateral fijo:** desde cualquier pantalla se llega a los 5 módulos con un clic.

## Tabla de navegación (de dónde → a dónde → con qué)
| # | De | A | Con qué elemento | Viene del user flow | Regla que cumple |
|---|---|---|---|---|---|
| 1 | Dashboard | Registrar prueba | Ítem «Registrar prueba» del menú lateral, o botón «+ Nueva evaluación» | Pasos 1 → 2 | Consistencia (H4) |
| 2 | Registrar prueba | Se queda en la misma pantalla | Mensaje de error bajo el campo; Guardar deshabilitado hasta completar | Rama «¿Datos válidos? → No» | Prevención de errores (H5) |
| 3 | Registrar prueba | Dashboard | Botón «Guardar» (solo con datos válidos) y mensaje de éxito | Pasos 5 → 6 | Visibilidad del estado (H1) |
| 4 | Registrar prueba | Dashboard | Botón «Cancelar» | Salida disponible en todo momento | Control y libertad del usuario (H3) |
| 5 | Cualquier pantalla | Cualquier módulo | Menú lateral fijo con el ítem activo resaltado | Todo el recorrido | Visibilidad del estado (H1) y consistencia (H4) |

**Nota:** con solo dos niveles de profundidad, el menú lateral con el ítem activo resaltado basta para
que el usuario sepa siempre dónde está y cómo volver.

## Comprobación
- [x] Cada flecha del user flow que cambia de pantalla tiene un elemento que la hace posible.
- [x] Se puede salir de cada pantalla (volver o cancelar).
- [x] El usuario sabe dónde está en todo momento.
- [x] Los nombres del menú son iguales a los títulos de las pantallas.
- [x] Está definido adónde regresa el usuario tras Guardar y tras Cancelar.
