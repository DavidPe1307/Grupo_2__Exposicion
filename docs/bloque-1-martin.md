# Bloque 1 · Requisitos, sitemap y navegación · Martín Palacios

> Documento completo: `docs/investigacion.md`. Este archivo es mi resumen para exponer y defender.

## Requisitos
- **Qué es:** algo que el usuario necesita poder hacer con el sistema. Se redacta desde el punto de vista del usuario, con un solo verbo, y se numera (R1, R2…).
- **Pregunta que responde:** ¿qué debe poder hacer el sistema?
- **Analogía:** la lista de necesidades de la casa (3 cuartos, 2 baños).
- **De qué depende:** de las historias de usuario, que ya son requisitos escritos desde el usuario.
- **Regla práctica:** un requisito, un verbo. Si lleva una «y», probablemente son dos.
- **Por qué se numeran:** para poder seguir cada requisito hasta el wireframe (trazabilidad).
- **En la Tarea 1:** R1 Llegar al formulario desde el dashboard · R2 Escribir quién fue evaluado y qué tarea hizo · R3 Escribir tiempo, errores, resultado y satisfacción · R4 Escribir observaciones · R5 Enterarse si dejó un dato obligatorio vacío o mal · R6 Guardar y ver que quedó guardado.

## Sitemap
- **Qué es:** un diagrama en forma de árbol que muestra qué pantallas existen y de cuál cuelga cada una.
- **Pregunta que responde:** ¿qué pantallas existen?
- **Analogía:** el índice de un libro.
- **De qué depende:** de los requisitos; cada requisito debe ocurrir en alguna pantalla.
- **Conceptos clave:** nivel 0 = raíz, nivel 1 = lo que se alcanza con un clic; pantallas hermanas; sitemap plano (pocos módulos) vs. profundo (muchas capas).
- **Simbología:** rectángulo = pantalla · resaltado = la que usa la tarea · borde punteado = reservada · línea continua = jerarquía · línea punteada = enlace de retorno · numeración 1.0, 3.1 = nivel y orden.
- **Reglas:** raíz arriba; cajas del mismo estilo; nombres cortos e iguales a los del menú; líneas que no se cruzan; leyenda incluida; cada requisito tiene una pantalla.
- **Error común:** incluir pantallas que ningún requisito pide, o dibujar flechas de recorrido (eso es del user flow).
- **En la Tarea 1:** 5 módulos a un clic desde el menú lateral (sitemap plano). R1 y R6 ocurren en el Dashboard (1.0); R2 a R5 en Registrar prueba (2.0). 3.1 Asistente IA está reservado para un sprint futuro.

## Navegación
- **Qué es:** los elementos visibles que permiten moverse entre las pantallas: menús, botones, enlaces, pestañas.
- **Pregunta que responde:** ¿cómo se llega de una pantalla a otra?
- **Analogía:** los letreros de un edificio.
- **De qué depende:** del sitemap y del user flow.
- **Tipos:** menú lateral, barra superior, pestañas, migas de pan, botones de acción, enlaces en el contenido.
- **Reglas:** consistencia; ubicación visible (ítem activo); pocos clics; siempre hay salida; nombres claros; definir adónde regresa el usuario tras cada acción.
- **Error común:** no definir adónde vuelve el usuario después de guardar o cancelar.
- **Heurísticas de Nielsen:** H1 visibilidad del estado, H3 control y libertad, H4 consistencia, H5 prevención de errores.
- **En la Tarea 1:** Dashboard → Registrar prueba con el menú lateral o «+ Nueva evaluación»; Registrar prueba → Dashboard con Guardar (datos válidos) o Cancelar; con error, el usuario se queda y corrige.

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
