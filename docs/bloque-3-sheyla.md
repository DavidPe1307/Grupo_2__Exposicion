# Bloque 3 · Wireframes, fidelidad y trazabilidad · Sheyla Pacha

> Documento completo: `docs/investigacion.md`. Este archivo es mi resumen.

## Wireframes
- **Qué es:** el dibujo esquemático de cada pantalla: qué elementos hay y dónde están.
- **Pregunta que responde:** ¿cómo se ve y qué contiene cada pantalla?
- **Analogía:** el plano de cada cuarto de la casa.
- **De qué depende:** del sitemap (qué pantallas), del user flow (orden y botones) y de los componentes (piezas).
- **Conceptos clave:** jerarquía visual (lo más importante se ve primero), alineación en cuadrícula, texto casi real (no «Lorem ipsum»), una acción principal por pantalla.
- **Reglas:** una acción principal por pantalla; campos relacionados agrupados; obligatorios marcados y ayuda bajo el campo; texto casi real; coherencia con el menú y el user flow.
- **Error común:** dibujar solo el camino feliz y olvidar la pantalla de error.

## Niveles de fidelidad
| | Lo-Fi (baja) | Mid-Fi (media) | Hi-Fi (alta) |
|---|---|---|---|
| Qué es | Bloques y líneas, solo estructura | Estructura detallada, sin diseño final | Casi idéntico al producto final |
| Color y texto | Blanco y grises; texto corto | Grises; texto real | Paleta y texto definitivos |
| Tiempo | Minutos por pantalla | Decenas de minutos | Horas |
| Costo de cambiar | Casi nada | Poco | Alto |
| Pregunta que responde | ¿Qué va y dónde? | ¿Se entiende y está bien organizado? | ¿Se ve y funciona como el real? |

Se empieza en baja fidelidad porque cambiar un rectángulo es fácil; cambiar un diseño pulido que tomó horas, no.

## Wireframe, mockup y prototipo
- **Wireframe:** dibujo estático de una pantalla (Lo-Fi o Mid-Fi) = el plano.
- **Mockup:** maqueta visual estática con el diseño final, sin interacción = la maqueta bonita.
- **Prototipo:** pantallas enlazadas en las que se puede hacer clic y navegar = la maqueta en la que puedes entrar y caminar.

## Wireframes de la Tarea 1 (un cuadro por momento del flujo)
1. **Dashboard (punto de partida)** · R1: menú lateral con «Dashboard» activo, tarjetas de conteo, problemas frecuentes, tabla de hallazgos y botón «+ Nueva evaluación».
2. **Formulario vacío** · R2, R3, R4: campos de identificación, métricas y observaciones; Cancelar y Guardar.
3. **Formulario con error** · R5: campo obligatorio vacío con borde rojo y mensaje bajo él; Guardar deshabilitado.
4. **Dashboard tras guardar** · R6: mensaje «Evaluación guardada» y contador de «Pruebas realizadas» de 12 a 13.

En los cuadros 3 y 4 hay marcas A y B (explicadas en la imagen). Las versiones Mid-Fi y Hi-Fi del repositorio son un adelanto de la Fase 2 (prototipo navegable), no parte de lo que pide esta fase.

## Trazabilidad
- **Qué es:** una tabla que sigue cada requisito por todos los productos: sitemap, navegación, user flow, componentes y wireframe.
- **Pregunta que responde:** ¿algún requisito se perdió en el camino?
- **Cómo se lee:** se empieza por el requisito, se sigue la fila y se termina en el cuadro del wireframe donde se puede ver y probar.
- **Prueba de fuego:** si una celda queda vacía, falta un artefacto. Si un wireframe o componente no tiene requisito, sobra o falta un requisito.
- **En la Tarea 1:** R5 → 2.0 Registrar prueba → error bajo el campo → rama «No» → mensaje de error → cuadro 3.

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