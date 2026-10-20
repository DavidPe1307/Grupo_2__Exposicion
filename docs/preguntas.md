# Banco de preguntas · Grupo 2

Preguntas de defensa (para el docente) y preguntas de Kahoot (para la clase), por bloque y en el orden de la exposición.
Kahoot: ver `src/fuentes-diagramas/KHOOT.md`.

# Bloque 1 · Requisitos, sitemap y navegación · Martín Palacios

## Preguntas de defensa
1. **¿Por qué menú lateral y no barra superior?** Son pocos módulos (5) que se usan con frecuencia; el menú queda siempre visible y el ítem resaltado dice dónde está el usuario (H1 y H4).
2. **¿Qué diferencia hay entre sitemap, navegación y user flow?** El sitemap dice qué pantallas hay; la navegación, con qué elemento se pasa de una a otra; el user flow, el recorrido de una persona en una tarea, incluyendo errores.
3. **Si un requisito con «y» son dos, ¿por qué R2, R3 y R6 llevan «y»?** R2 y R3 usan el mismo verbo (escribir) sobre campos del mismo bloque del formulario. En R6 la acción es guardar; «ver que quedó guardado» es la confirmación de esa misma acción (H1).
4. **¿Qué diferencia hay entre R4 y el módulo Observaciones (3.0)?** R4 es el campo de observaciones del evaluador dentro del formulario; el módulo 3.0 es una pantalla aparte del proyecto. *(Ajustar a lo que realmente hace su módulo.)*

## Preguntas de Kahoot (4)
1. **¿Cuál es la regla práctica para redactar un requisito?**
   a) Mínimo tres verbos · b) Incluir el color del botón · c) **Un requisito, un verbo** · d) Escribirlo desde el punto de vista del programador
   *Correcta: c.*
2. **¿Qué pregunta responde el sitemap?**
   a) ¿Qué camino sigue el usuario? · b) **¿Qué pantallas existen?** · c) ¿Cómo se ve cada pantalla? · d) ¿Con qué piezas se arma?
   *Correcta: b.*
3. **¿Cuál es un error común al dibujar un sitemap?**
   a) Numerar las pantallas · b) Incluir una leyenda · c) Usar nombres cortos · d) **Dibujar flechas de recorrido**
   *Correcta: d. El recorrido pertenece al user flow.*
4. **En la Tarea 1, ¿adónde regresa el usuario al guardar o cancelar?**
   a) **Al Dashboard** · b) Al formulario vacío · c) Al Product Backlog · d) Sale del sistema
   *Correcta: a.*

# Bloque 2 · User flow y componentes · David Pérez

## Preguntas de defensa
1. **¿Cuál es la diferencia entre sitemap y user flow?** El sitemap muestra todas las pantallas que existen y de cuál cuelga cada una; el user flow muestra el recorrido de una persona en una sola tarea, con decisiones y errores.
2. **¿Por qué el user flow tiene rama de error y no una rama «Cancelar»?** La rama de error es parte del camino de la tarea (R5). «Cancelar» es una salida disponible siempre, y se define en la navegación (H3), así el flujo no se llena de flechas.
3. **¿Por qué el campo de texto es una molécula y no un átomo?** Porque junta etiqueta, caja, ayuda y mensaje de error; el átomo sería solo la caja.
4. **¿Por qué «Guardar» tiene estado deshabilitado?** Para prevenir errores (H5): no se puede enviar el formulario incompleto. Para que no confunda, el formulario dice «Completa los campos obligatorios (*) antes de guardar».

## Preguntas de Kahoot (4)
1. **¿Qué forma se usa en un user flow para una decisión con dos salidas (Sí / No)?**
   a) Un óvalo · b) Un rectángulo · c) **Un rombo** · d) Un círculo numerado
   *Correcta: c.*
2. **¿Qué debe hacer el camino de error de un user flow?**
   a) Terminar el recorrido · b) **Regresar a un paso anterior** · c) Salir del sistema · d) Ocultarse
   *Correcta: b. El usuario nunca queda sin salida.*
3. **En Atomic Design, ¿qué es un campo de texto con etiqueta, ayuda y error?**
   a) Un átomo · b) **Una molécula** · c) Un organismo · d) Una pantalla
   *Correcta: b.*
4. **¿Qué regla justifica que exista un componente?**
   a) Que se vea bonito · b) Que lo pida el cliente por correo · c) **Que responda a un requisito** · d) Que sea de color morado
   *Correcta: c.*

# Bloque 3 · Wireframes, fidelidad y trazabilidad · Sheyla Pacha

## Preguntas de defensa
1. **¿Por qué empezar en baja fidelidad?** Porque cambiar un bloque gris cuesta casi nada y rediseñar algo pulido cuesta horas; en esta etapa solo se decide qué va y dónde.
2. **¿Por qué incluyen Mid-Fi y Hi-Fi si el tema es Lo-Fi?** Como adelanto de la siguiente fase, para mostrar cómo evoluciona la misma pantalla. El producto de esta fase son los wireframes Lo-Fi.
3. **¿Por qué el formulario muestra una escala de severidad si no hay un campo de severidad?** Es un banner informativo para que el evaluador no dependa de su memoria. *(Si lo quitan del wireframe, cambien esta respuesta.)*
4. **¿Por qué el participante se registra como código anónimo?** Para no guardar datos personales de los evaluados (privacidad).

## Preguntas de Kahoot (4)
1. **¿Por qué se empieza dibujando en baja fidelidad?**
   a) Porque se ve más bonito · b) **Porque cambiar un bloque es casi gratis** · c) Porque ya incluye la paleta final · d) Porque es lo que usa el cliente
   *Correcta: b.*
2. **¿Qué es un mockup?**
   a) Un conjunto de pantallas enlazadas con clics · b) Un boceto a mano · c) **Una maqueta visual estática con el diseño final** · d) Un diagrama de flujo
   *Correcta: c.*
3. **¿Cuál NO es una regla de los wireframes?**
   a) Una acción principal por pantalla · b) Marcar los campos obligatorios · c) Coherencia con el menú y el user flow · d) **Usar «Lorem ipsum» en todos los textos**
   *Correcta: d. Se usa texto casi real.*
4. **En la matriz de trazabilidad, una celda vacía significa:**
   a) **Que falta un artefacto** · b) Que el requisito no es importante · c) Que no se necesita wireframe · d) Que la tarea terminó
   *Correcta: a.*
