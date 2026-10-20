# Borrador · Componentes · Tarea 1 «Registrar evaluación»

> Lista de trabajo previa al inventario final (`prototipos/05-componentes.md`).

## Lista inicial (sin clasificar)
Menú lateral, formulario, campo de texto, lista desplegable, selector 1–5, tarjeta de conteo,
botón + Nueva evaluación, botón Guardar, botón Cancelar, mensaje de error, mensaje de éxito.

## Clasificación (Atomic Design)
- Átomos: botones (+ Nueva evaluación, Guardar, Cancelar), mensaje de error, mensaje de éxito
- Moléculas: campo de texto con etiqueta/ayuda/error, lista desplegable, selector 1–5, tarjeta de conteo
- Organismos: menú lateral, formulario de registro

## Dudas y decisiones
- Duda: ¿el campo de texto es átomo o molécula? Decisión: molécula, porque junta etiqueta, caja, ayuda y error.
- Duda: ¿Cancelar es un requisito? Decisión: no, es la salida del usuario (H3).
- Los filtros y la tabla de hallazgos del Dashboard no vienen de R1–R6: se anotan como contexto, no como componentes.

## Estados pendientes de definir
Campo: normal, foco, error. Guardar: normal, foco, deshabilitado.
