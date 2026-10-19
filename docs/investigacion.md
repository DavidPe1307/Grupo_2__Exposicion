# Prototipos y wireframes: de requisitos a arquitectura, flujo y wireframe

Interacción Humano-Computador · APE 4, Fase 1 · Grupo 2 (5.º Software, paralelo B)
Universidad Técnica de Ambato · FISEI
Integrantes: Sheyla Pacha, Martín Palacios, David Pérez
Proyecto de aplicación: Usability Test Dashboard 2.0 · Tarea 1 «Registrar evaluación»

---

# PARTE 1. CONCEPTOS

## El proceso completo

Antes de programar una aplicación se planea en papel qué pantallas tendrá, cómo se pasa de una a otra y cómo se ve cada una. Ese planeamiento se hace en un orden, y cada paso sale del anterior:

Requisitos → Sitemap → Navegación → User flow → Componentes → Wireframes → Trazabilidad

Piensa en construir una casa. No empiezas poniendo ladrillos:

| Paso del proceso | Pregunta que responde | Analogía de la casa |
|---|---|---|
| Requisitos | ¿Qué debe poder hacer el sistema? | La lista de necesidades (3 cuartos, 2 baños) |
| Sitemap | ¿Qué pantallas existen y cómo se agrupan? | La lista de habitaciones |
| Navegación | ¿Cómo se pasa de una pantalla a otra? | Los pasillos y las puertas |
| User flow | ¿Qué camino sigue una persona para lograr una tarea? | El recorrido de la puerta de entrada a la cocina |
| Componentes | ¿Con qué piezas se arma cada pantalla? | Los tipos de ventanas, puertas e interruptores |
| Wireframes | ¿Cómo se ve y qué contiene cada pantalla? | El plano de cada cuarto por dentro |

Los componentes y los wireframes se definen casi al mismo tiempo: al dibujar una pantalla aparecen piezas nuevas, y al listar piezas se ajusta el dibujo.

## Punto de partida: los requisitos

Un requisito es algo que el usuario necesita poder hacer con el sistema. Se redacta desde el punto de vista del usuario y con un solo verbo (ingresar, validar, guardar). Las historias de usuario ya son requisitos escritos de esa forma; aquí se convierten en acciones concretas y se numeran (R1, R2, R3…), porque esos números permiten seguir cada requisito hasta el wireframe.

Regla práctica: un requisito, un verbo. Si el requisito lleva una «y», probablemente son dos.

---

## 1. Sitemap

**Qué es.** Un diagrama en forma de árbol que muestra qué pantallas existen y de cuál cuelga cada una.

**Pregunta que responde.** ¿Qué pantallas existen?

**Analogía.** El índice de un libro: dice qué capítulos hay y cómo se organizan.

**De qué depende.** De los requisitos: cada requisito debe ocurrir en alguna pantalla.

**Lo que se debe saber antes.**
- Nivel y profundidad: el nivel 0 es la raíz (el sistema completo) y el nivel 1 es lo que se alcanza con un clic desde el inicio.
- Pantallas «hermanas»: las que están en la misma fila y tienen el mismo nivel de importancia.
- Sitemap plano y sitemap profundo: es plano cuando hay pocos módulos al mismo nivel, y profundo cuando hay muchas capas.
- Simbología habitual:

| Símbolo | Significa |
|---|---|
| Rectángulo | Una pantalla o página |
| Rectángulo resaltado | Una pantalla que usa la tarea que se está explicando |
| Rectángulo con borde punteado | Pantalla reservada o futura |
| Línea continua | Relación jerárquica (de aquí cuelga esto) |
| Línea punteada | Enlace secundario o de retorno |
| Numeración (1.0, 3.1) | Nivel y orden (3.1 es hijo de 3.0) |

**Reglas básicas.**
1. La raíz va arriba y cada fila hacia abajo es un nivel.
2. Todas las cajas tienen el mismo tamaño y estilo.
3. Los nombres son cortos e iguales a los del menú.
4. Las líneas no se cruzan.
5. Se incluye una leyenda con el significado de cada símbolo.
6. Cada requisito tiene una pantalla.

**Pasos para definirlo.**
1. Lista los requisitos.
2. Para cada uno pregunta: ¿en qué pantalla ocurre?
3. Agrupa las pantallas del mismo tema bajo una sección.
4. Ordénalas como árbol y numéralas.
5. Revisa la profundidad (lo importante a máximo 3 clics) y que ningún requisito quede sin pantalla.

**Error común.** Incluir pantallas que ningún requisito pide, o dibujar flechas de recorrido en el sitemap (eso pertenece al user flow).

**Tip.** Escribe los requisitos en una columna y, al lado, la pantalla donde ocurre cada uno. Esa tabla ya es el sitemap en borrador; solo falta ordenarla como árbol.

---

## 2. Navegación

**Qué es.** Los elementos visibles que permiten moverse entre las pantallas del sitemap: menús, botones, enlaces, pestañas.

**Pregunta que responde.** ¿Cómo se llega de una pantalla a otra?

**Analogía.** Los letreros de un edificio: te dicen dónde está cada cosa y cómo ir.

**De qué depende.** Del sitemap, que dice entre qué pantallas hay que poder moverse, y del user flow, que dice qué movimientos hace el usuario en cada tarea.

**Lo que se debe saber antes.**

| Tipo de navegación | Qué es | Cuándo conviene |
|---|---|---|
| Menú lateral | Lista fija a la izquierda | Pocas secciones grandes que se usan seguido |
| Barra superior | Menú horizontal arriba | Sistemas simples, pocas secciones |
| Pestañas | Cambias de vista dentro de una misma pantalla | Contenidos relacionados de una misma sección |
| Migas de pan | Ruta de dónde estás (Inicio > Sección > Pantalla) | Cuando hay varios niveles de profundidad |
| Botones de acción | Guardar, Cancelar, «+ Nueva evaluación» | Para avanzar o retroceder dentro de una tarea |
| Enlaces en el contenido | Texto o filas que llevan al detalle | Listas y tablas |

Heurísticas de Nielsen relacionadas: H1 visibilidad del estado del sistema, H3 control y libertad del usuario, H4 consistencia y estándares, H5 prevención de errores.

**Reglas básicas.**
1. Consistencia: el menú está en el mismo lugar y se ve igual en todas las pantallas.
2. Ubicación visible: el usuario siempre sabe dónde está (ítem activo resaltado, título de la pantalla).
3. Pocos clics: lo más usado queda a uno o dos clics.
4. Siempre hay salida: cada pantalla permite volver o cancelar.
5. Nombres claros y cortos, los mismos en el menú, en el título y en la documentación.
6. Se define adónde regresa el usuario después de cada acción importante (guardar, cancelar).

**Pasos para definirla.**
1. Toma cada flecha del user flow que cambia de pantalla.
2. Para cada una pregunta: ¿con qué elemento lo hace el usuario?
3. Escribe una tabla de dónde → a dónde → con qué.
4. Define el regreso después de cada acción.
5. Revisa que no queden pantallas sin entrada ni sin salida.

**Error común.** Dejar sin definir adónde vuelve el usuario después de guardar o cancelar.

---

## 3. User flow

**Qué es.** El recorrido paso a paso que sigue una persona para lograr una tarea concreta, incluyendo lo que pasa si algo sale mal.

**Pregunta que responde.** ¿Qué camino sigue el usuario?

**Analogía.** El sitemap es el mapa de toda la ciudad; el user flow es la ruta de tu casa a la universidad.

**De qué depende.** De los requisitos y del sitemap, y de la tarea que se elija mostrar.

**Lo que se debe saber antes.**

| Forma | Significa |
|---|---|
| Óvalo | Inicio o fin del recorrido |
| Rectángulo | Un paso: una pantalla que ve el usuario |
| Rectángulo redondeado | Una acción del usuario o del sistema |
| Rombo | Una decisión con dos o más salidas (Sí / No) |
| Flecha | El sentido del recorrido |
| Texto sobre la flecha | La condición que activa esa salida |

Camino feliz: el recorrido en el que todo sale bien. Camino de error: el recorrido que se toma cuando un dato es inválido o una acción falla.

**Reglas básicas.**
1. Un solo inicio y uno o más finales.
2. Los pasos van en orden, de izquierda a derecha.
3. Todo rombo tiene al menos dos salidas con su etiqueta.
4. El camino de error regresa a un paso anterior: el usuario nunca queda sin salida.
5. Cada recuadro es algo que se puede dibujar (una pantalla) o hacer (una acción).

**Pasos para definirlo.**
1. Escribe la tarea en una frase.
2. Dibuja solo el camino feliz.
3. En cada paso pregunta: ¿qué puede salir mal aquí?
4. Agrega esas ramas.
5. Termina siempre con lo que ve el usuario.
6. Recórrelo con el dedo sobre los wireframes para confirmar que no te saltas nada.

**Error común.** Un nodo final que no corresponde a ninguna pantalla real.

**Tip.** Dibuja primero el camino feliz de corrido y después agrega los errores como ramas. Hacerlo al revés enreda el diagrama.

---

## 4. Componentes

**Qué es.** Las piezas de interfaz reutilizables con las que se arman las pantallas: botón, campo de texto, tarjeta, menú, tabla.

**Pregunta que responde.** ¿Con qué piezas se arma cada pantalla?

**Analogía.** Los bloques de Lego: se usan los mismos bloques en muchas pantallas y por eso todo se ve igual y es más fácil de construir.

**De qué depende.** De los wireframes y de los requisitos. Se definen junto con los wireframes: al dibujar una pantalla se ven las piezas que necesita.

**Lo que se debe saber antes.**

Atomic Design organiza los componentes por tamaño:

| Nivel | Qué es | Ejemplo |
|---|---|---|
| Átomo | La pieza más pequeña, sola | Botón, caja de texto, etiqueta, mensaje |
| Molécula | Varios átomos con un propósito | Campo completo: etiqueta + caja + ayuda + error |
| Organismo | Un bloque grande de la pantalla | Menú lateral, formulario completo, tabla |
| Plantilla | La estructura vacía de una pantalla | Menú a la izquierda, encabezado y zona de contenido |
| Página | La plantilla con contenido real | La pantalla terminada |

Los estados: un componente no solo existe «normal». Puede estar en foco, deshabilitado, con error, vacío o en éxito.

**Reglas básicas.**
1. Si se repite, es componente (aparece en varias pantallas o varias veces en una).
2. Un nombre, una función: no hay dos nombres para la misma pieza.
3. Cada componente justifica su existencia con un requisito.
4. Consistencia: la misma pieza se ve y se comporta igual en todas partes.
5. No se crea un componente para algo que aparece una sola vez sin motivo.

**Pasos para definirlos.**
1. Abre el wireframe de la pantalla.
2. Recórrelo de arriba hacia abajo y anota cada elemento visible.
3. Agrupa los repetidos y dales un nombre.
4. Clasifícalos en átomo, molécula u organismo.
5. Define los estados que necesita cada uno.
6. Anota el requisito que cubre cada uno.

**Error común.** Piezas que ningún requisito pidió, o la misma pieza con dos nombres distintos.

---

## 5. Wireframes y niveles de fidelidad

**Qué es.** El dibujo esquemático de cada pantalla: qué elementos hay y en qué lugar están.

**Pregunta que responde.** ¿Cómo se ve y qué contiene cada pantalla?

**Analogía.** El plano de cada cuarto de la casa.

**De qué depende.** Del sitemap (qué pantallas se dibujan), del user flow (en qué orden y con qué botones) y de los componentes (con qué piezas).

**Lo que se debe saber antes.**
- Jerarquía visual: lo más importante se ve primero (título, acción principal).
- Alineación y cuadrícula: los elementos se acomodan en columnas y filas ordenadas.
- Texto casi real: se escriben textos verosímiles, no «Lorem ipsum».
- Una acción principal por pantalla.

### Niveles de fidelidad

La fidelidad es qué tanto se parece el dibujo al producto final. Se avanza de lo rápido y barato a lo detallado y costoso.

| | Baja fidelidad (Lo-Fi) | Media fidelidad (Mid-Fi) | Alta fidelidad (Hi-Fi) |
|---|---|---|---|
| Qué es | Bloques y líneas, solo estructura | Estructura detallada, sin diseño visual final | Casi idéntico al producto final |
| Color | No, blanco y grises | Grises o un tono neutro | Paleta definitiva |
| Texto | Genérico o corto | Real | Real y definitivo |
| Detalle | Mínimo | Jerarquía, espaciado, estados básicos | Tipografías, imágenes, íconos, todos los estados |
| Interactivo | No | A veces | Normalmente sí (clicable) |
| Tiempo | Minutos por pantalla | Decenas de minutos | Horas |
| Costo de cambiar | Casi nada | Poco | Alto |
| Pregunta que responde | ¿Qué va y dónde? | ¿Se entiende y está bien organizado? | ¿Se ve bien y funciona como el real? |
| Se usa para | Decidir la estructura | Validar contenido y organización | Pruebas realistas, aprobación y guía para programar |

Se empieza en baja fidelidad porque cambiar un rectángulo es fácil; cambiar un diseño pulido que ya tomó horas, no.

### Wireframe, mockup y prototipo

- Wireframe: el dibujo estático de una pantalla (Lo-Fi o Mid-Fi).
- Mockup: la maqueta visual estática con el diseño final, sin interacción.
- Prototipo: un conjunto de pantallas enlazadas con las que se puede hacer clic y navegar, para simular el uso.

Para recordarlo: wireframe = plano; mockup = maqueta bonita; prototipo = maqueta en la que puedes entrar y caminar.

**Reglas básicas.**
1. Una acción principal por pantalla, la más visible.
2. Los campos relacionados se agrupan.
3. Los campos obligatorios se marcan y la ayuda va debajo del campo.
4. Se usa texto casi real.
5. Hay coherencia con el menú y con el user flow.

**Pasos para definirlos.**
1. Haz un cuadro por cada momento del user flow.
2. Coloca la estructura: menú, encabezado, contenido y acciones.
3. Coloca los componentes.
4. Escribe el texto real.
5. Dibuja los estados que importan: error, vacío, éxito.
6. Revisa cada cuadro contra el user flow y los requisitos.

**Error común.** Dibujar solo el camino feliz y olvidar la pantalla de error.

---

## Resumen de la Parte 1

| Concepto | Pregunta que responde | De qué depende |
|---|---|---|
| Sitemap | ¿Qué pantallas existen? | Requisitos |
| Navegación | ¿Cómo se llega de una a otra? | Sitemap y user flow |
| User flow | ¿Qué camino sigue el usuario? | Requisitos y sitemap |
| Componentes | ¿Con qué piezas se arma cada pantalla? | Wireframes y requisitos |
| Wireframes | ¿Cómo se ve cada pantalla? | Sitemap, user flow y componentes |

---

# PARTE 2. EJEMPLO PRÁCTICO: TAREA 1 «REGISTRAR EVALUACIÓN»

## Qué significa «definir sitemap, user flow, navegación, componentes y wireframes de baja fidelidad» aplicado a la Tarea 1

La frase pide cinco productos. Cada uno responde una pregunta distinta sobre la misma tarea: «Ana termina una prueba de usabilidad y quiere guardar sus resultados».

Ana es la evaluadora de usabilidad del proyecto Usability Test Dashboard 2.0. Pone a un participante a usar una aplicación y anota cuánto tardó, cuántos errores cometió, si logró la tarea y qué tan satisfecho quedó. Después entra al sistema para guardar esos datos.

Como punto de partida están los requisitos de la Tarea 1, que salen de las historias de usuario del proyecto (HU-01, HU-02, HU-10 y HU-11):

| ID | Ana debe poder... |
|---|---|
| R1 | Llegar al formulario desde el dashboard |
| R2 | Escribir quién fue evaluado y qué tarea hizo |
| R3 | Escribir tiempo, errores, resultado y satisfacción |
| R4 | Escribir sus observaciones |
| R5 | Enterarse si dejó un dato obligatorio mal o vacío |
| R6 | Guardar y ver que quedó guardado |

Los cinco productos son la forma de convertir esa lista en algo que se pueda construir.

---

## 1. Sitemap: ¿qué pantallas hacen falta?

Tomas los requisitos y te preguntas: «¿en qué pantalla ocurre cada uno?».

- R1 ocurre en el Dashboard (desde ahí se entra al formulario).
- R2, R3, R4 y R5 ocurren en Registrar prueba (el formulario).
- R6 ocurre en el Dashboard otra vez (ahí se confirma que quedó guardado).

Entonces, para la Tarea 1 solo necesitas dos pantallas. El sitemap completo del proyecto muestra además las otras tres (Observaciones, Product Backlog y Tablero SCRUM), pero esta tarea no las usa, así que se resaltan solo las dos que participan.

```
Usability Test Dashboard 2.0   (nivel 0 · raíz)
├─ 1.0 Dashboard de resultados      ◄ Tarea 1 (HU-02, HU-11)
├─ 2.0 Registrar prueba             ◄ Tarea 1 (HU-01, HU-10)
├─ 3.0 Observaciones
│      └─ 3.1 Asistente IA          (reservado · Sprint 5)
├─ 4.0 Product Backlog              (HU-07)
└─ 5.0 Tablero SCRUM                (HU-08)
```

Cómo se lee:
- Es un sitemap plano: los 5 módulos están al mismo nivel y se llega a cualquiera con un clic desde el menú lateral. Eso se justifica porque son pocos módulos y todos se usan con frecuencia.
- Una línea punteada de retorno une Registrar prueba con el Dashboard: al guardar o cancelar, el usuario vuelve ahí.
- La pantalla 3.1 aparece con borde punteado porque está reservada para un sprint futuro.

Cómo se hizo: se escribió cada requisito junto a la pantalla donde ocurre, se agruparon las pantallas del mismo tema, se ordenaron como árbol y se numeraron.

---

## 2. Navegación: ¿cómo llega Ana de una pantalla a otra?

El sitemap dice qué pantallas hay; la navegación dice con qué botones o menús se pasa de una a otra. En la Tarea 1:

- Del Dashboard al formulario: con el menú lateral («Registrar prueba») o con el botón «+ Nueva evaluación».
- Del formulario de vuelta al Dashboard: con Guardar (cuando todo está bien) o con Cancelar.
- Entre cualquier módulo: con el menú lateral fijo, que muestra resaltado el ítem donde estás.

Aquí también se define adónde vuelve el usuario después de cada acción, que es lo que más suele quedar sin decidir.

| De | A | Con qué elemento | Regla que cumple |
|---|---|---|---|
| Dashboard | Registrar prueba | Ítem «Registrar prueba» del menú lateral, o botón «+ Nueva evaluación» | Consistencia (H4) |
| Registrar prueba | Se queda en la misma pantalla | Mensaje de error bajo el campo; Guardar deshabilitado hasta completar | Prevención de errores (H5) |
| Registrar prueba | Dashboard | Botón «Guardar» (solo con datos válidos) y mensaje de éxito | Visibilidad del estado (H1) |
| Registrar prueba | Dashboard | Botón «Cancelar» | Control y libertad del usuario (H3) |
| Cualquier pantalla | Cualquier módulo | Menú lateral fijo con el ítem activo resaltado | Visibilidad del estado (H1) y consistencia (H4) |

Como la estructura tiene solo dos niveles de profundidad, el menú lateral con el ítem activo resaltado alcanza para que el usuario sepa siempre dónde está.

---

## 3. User flow: ¿qué camino sigue Ana para lograr la tarea?

Es el recorrido paso a paso, incluyendo qué pasa si algo sale mal:

Inicio → Dashboard → Registrar prueba → Llenar campos → ¿Datos válidos?

- Sí → Guardar → Dashboard con mensaje de éxito → Fin.
- No → Mostrar error bajo el campo → Ana corrige y vuelve a «Llenar campos».

En el diagrama, los rectángulos son las pantallas (Dashboard, Registrar prueba, Dashboard con mensaje de éxito) y las formas redondeadas son las acciones (Llenar campos, Guardar, Mostrar error). El rombo es la decisión «¿Datos válidos?».

Fíjate cómo cada requisito aparece en el flujo:
- R1 son los dos primeros pasos (Dashboard → Registrar prueba).
- R2, R3 y R4 son el paso «Llenar campos».
- R5 es la rama de error.
- R6 es el final: Guardar y el Dashboard con mensaje de éxito.

Paso a paso del recorrido:
1. Dashboard: Ana ve el resumen (conteos y filtros).
2. Registrar prueba: abre el formulario desde el menú o con «+ Nueva evaluación».
3. Llenar campos: escribe identificación, métricas y observaciones.
4. ¿Datos válidos?: el sistema revisa los campos obligatorios.
5. Guardar: el botón se habilita solo cuando todo es válido.
6. Dashboard con mensaje de éxito: aparece «Evaluación guardada» y el contador de pruebas realizadas sube.

---

## 4. Componentes: ¿con qué piezas se arma el formulario?

Miras la pantalla del formulario y listas las piezas que la componen. Son las que luego se programan una sola vez y se reutilizan:

| Componente | Nivel | Estados que necesita | Requisito |
|---|---|---|---|
| Menú lateral | Organismo | Normal, ítem activo | R1 |
| Formulario de registro | Organismo | Normal, con error | R2, R3, R4, R5 |
| Campo de texto con etiqueta, ayuda y error | Molécula | Normal, foco, error | R2, R4 |
| Lista desplegable («Resultado de la tarea») | Molécula | Normal, foco, error | R3 |
| Selector 1–5 («Satisfacción») | Molécula | Normal, seleccionado | R3 |
| Tarjeta de conteo («Pruebas realizadas») | Molécula | Normal | R6 |
| Botón «+ Nueva evaluación» | Átomo | Normal, foco | R1 |
| Botón «Guardar» | Átomo | Normal, foco, deshabilitado | R5, R6 |
| Botón «Cancelar» | Átomo | Normal, foco | Salida del usuario (H3) |
| Mensaje de error bajo el campo | Átomo | Visible, oculto | R5 |
| Mensaje de éxito | Átomo | Visible, oculto | R6 |

Así se ve que cada pieza existe por un requisito: ninguna sobra. Los valores exactos de color y borde de cada estado están definidos en la guía de estilo del proyecto.

---

## 5. Wireframes de baja fidelidad: ¿cómo se ve cada pantalla?

Son los dibujos simples de cada pantalla, con cajas y texto, sin colores ni diseño final. «Baja fidelidad» quiere decir que se parecen poco al producto terminado a propósito, porque en esta etapa solo decides qué va y dónde.

Para contar toda la Tarea 1 hay un dibujo por cada momento del flujo:

| # | Momento | Requisito | Qué muestra |
|---|---|---|---|
| 1 | Dashboard (punto de partida) | R1 | Menú lateral con «Dashboard» activo, tres tarjetas de conteo (pruebas realizadas, hallazgos registrados, severidad promedio), problemas frecuentes, tabla de hallazgos y el botón «+ Nueva evaluación» |
| 2 | Formulario vacío | R2, R3, R4 | Campos de identificación, métricas (tiempo, errores, resultado, satisfacción) y observaciones; botones Cancelar y Guardar |
| 3 | Formulario con un error visible | R5 | Un campo obligatorio vacío con borde de error y el mensaje «Campo obligatorio» bajo él; Guardar deshabilitado |
| 4 | Dashboard después de guardar | R6 | Mensaje «Evaluación guardada» y la tarjeta «Pruebas realizadas» con el contador aumentado en uno |

Qué observar en ellos:
- El menú lateral está igual en todas las pantallas y resalta el módulo activo (consistencia, H4).
- Los campos obligatorios llevan asterisco y la ayuda aparece debajo de cada campo.
- La escala de severidad se muestra en el encabezado del formulario para no depender de la memoria del evaluador.
- Cancelar y Guardar están abajo a la derecha, donde se espera la acción final, y Guardar es la acción principal.
- Cada nodo del user flow tiene su propio cuadro: si no se puede dibujar, el nodo no está bien definido.

---

## Cómo se une todo

Cada producto sale del anterior, y en todos reaparecen los mismos requisitos:

| Requisito | Sitemap | Navegación | User flow | Componentes | Wireframe |
|---|---|---|---|---|---|
| R1 | Dashboard → Registrar prueba | Menú / «+ Nueva evaluación» | Pasos 1 y 2 | Menú lateral; botón «+ Nueva evaluación» | Cuadro 1 |
| R2 | Registrar prueba | (ya estás ahí) | Llenar campos | Campo de texto; formulario | Cuadro 2 |
| R3 | Registrar prueba | (ya estás ahí) | Llenar campos | Campo; lista desplegable; selector 1–5 | Cuadro 2 |
| R4 | Registrar prueba | (ya estás ahí) | Llenar campos | Campo de texto (área) | Cuadro 2 |
| R5 | Registrar prueba | Error bajo el campo; Guardar deshabilitado | ¿Datos válidos? → error | Mensaje de error; botón Guardar (deshabilitado) | Cuadro 3 |
| R6 | Dashboard | Guardar → Dashboard | Guardar → éxito | Botón Guardar; mensaje de éxito; tarjeta de conteo | Cuadro 4 |

Esta tabla es lo que significa «pasar de requisitos a arquitectura, flujo y wireframe»: un mismo requisito que puedes seguir de punta a punta sin huecos.

---

## Cómo repetir el ejercicio con tu propio caso

1. Escribe de 4 a 6 requisitos, uno por verbo.
2. Dibuja el sitemap y numéralo.
3. Define la navegación en una tabla de dónde → a dónde → con qué.
4. Traza el user flow con una rama de error.
5. Lista los componentes con su nivel y sus estados.
6. Dibuja un cuadro de wireframe por cada momento del flujo.
7. Arma la tabla de trazabilidad.

## Comprobación final

- Todo requisito tiene pantalla, flujo y wireframe (ninguna celda vacía en la trazabilidad).
- Todo wireframe corresponde a algún requisito (nada sobra).
- Todo componente de la tabla aparece dibujado en un cuadro.
- Todo nodo del user flow tiene su cuadro de wireframe.
- Los nombres son iguales en el sitemap, el menú y los títulos de las pantallas.

## Continuidad con el proyecto

Esta tarea es una de las tres tareas críticas del Sprint 1 del Usability Test Dashboard 2.0. El proyecto completo incluye wireframes Lo-Fi de cinco pantallas (Dashboard de resultados, Registrar evaluación, Observaciones con espacio reservado para el Asistente IA, Product Backlog y Tablero SCRUM), el user flow de las tres tareas críticas (registrar evaluación, ver problemas frecuentes, planificar y mover tareas) y una guía de estilo que define el siguiente paso hacia media y alta fidelidad.