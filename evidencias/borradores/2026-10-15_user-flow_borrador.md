# Borrador · User flow · Tarea 1 «Registrar evaluación»

> Notas de trabajo previas al diagrama final (`prototipos/04-user-flow.png`).

## Primer intento (solo camino feliz)
Inicio → Dashboard → Registrar prueba → Llenar campos → Guardar → Dashboard → Fin

## Problemas que vi
- No decía qué pasa si un campo obligatorio queda vacío.
- Faltaba el mensaje de éxito después de guardar.
- «Guardar» no tenía condición: debía haber una decisión antes.

## Segundo intento (con rama de error)
Inicio → Dashboard → Registrar prueba → Llenar campos → ¿Datos válidos?
- Sí → Guardar → Dashboard + mensaje de éxito → Fin
- No → Mostrar error bajo el campo → vuelve a Llenar campos

## Relación con los requisitos
- R1: pasos 1 y 2 (llegar al formulario)
- R2 a R4: Llenar campos
- R5: rama «No» (error)
- R6: Guardar y mensaje de éxito

## Dudas que quedaron
- ¿Se dibuja la rama «Cancelar»? Decisión: no, se define en la navegación (H3).
- ¿El nodo Fin corresponde a una pantalla real? Sí: el Dashboard tras guardar.
