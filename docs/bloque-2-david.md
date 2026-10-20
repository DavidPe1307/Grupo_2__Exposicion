# Bloque 2 · User flow y componentes · David Pérez

> Documento completo: `docs/investigacion.md`. Este archivo es mi resumen para exponer y defender.

## User flow
- **Qué es:** el recorrido paso a paso que sigue una persona para lograr UNA tarea, incluyendo qué pasa si algo sale mal.
- **Pregunta que responde:** ¿qué camino sigue el usuario para lograr su tarea?
- **Analogía:** el recorrido de la puerta de entrada a la cocina.
- **De qué depende:** del sitemap (las pantallas por las que pasa) y de la navegación (con qué elementos se mueve).
- **Simbología:** óvalo = inicio/fin · rectángulo = pantalla · forma redondeada = acción · rombo = decisión (Sí / No) · flecha morada = camino feliz · flecha roja = camino de error · círculo numerado = número de paso.
- **Reglas:** un solo inicio y uno o más finales; los pasos van en orden; toda decisión tiene al menos dos salidas etiquetadas; el camino de error regresa a un paso anterior (el usuario nunca queda sin salida); es el recorrido de UNA tarea.
- **Error común:** dibujar solo el camino feliz y olvidar la rama de error. En mi borrador (`evidencias/borradores/2026-10-15_user-flow_borrador.md`) me pasó: faltaba la decisión antes de Guardar y el mensaje de éxito.
- **En la Tarea 1:** Inicio → Dashboard → Registrar prueba → Llenar campos → ¿Datos válidos? → (Sí) Guardar → Dashboard + éxito → Fin · (No) Mostrar error bajo el campo → vuelve a Llenar campos.

## Componentes
- **Qué es:** las piezas reutilizables con las que se arma cada pantalla.
- **Pregunta que responde:** ¿con qué piezas se arma cada pantalla?
- **Analogía:** los tipos de ventanas, puertas e interruptores de la casa.
- **De qué depende:** de los requisitos (cada componente justifica su existencia con uno) y se define junto con los wireframes.
- **Atomic Design:** átomo (botón, mensaje) → molécula (campo con etiqueta, ayuda y error) → organismo (menú lateral, formulario).
- **Estados:** cada componente se define con sus estados (campo: normal, foco, error; Guardar: normal, foco, deshabilitado).
- **Reglas:** si se repite, es componente; un nombre, una función; cada componente tiene un requisito; consistencia en todas partes; no crear componentes de uso único sin motivo.
- **En la Tarea 1:** 11 componentes (5 átomos —3 botones y 2 mensajes—, 4 moléculas y 2 organismos; «Cancelar» responde a H3, no a un requisito). Detalle en `prototipos/05-componentes.md`.

## Cómo se une con el resto
El user flow toma las pantallas del sitemap y los elementos de la navegación y los ordena en el tiempo. Los componentes salen de lo que ese recorrido necesita en cada pantalla, y los wireframes los colocan. Cada nodo del flujo tiene su cuadro de wireframe (`prototipos/07-trazabilidad.md`).

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
