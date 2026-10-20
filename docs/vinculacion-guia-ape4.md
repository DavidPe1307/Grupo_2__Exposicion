# Vinculación con la Guía de Práctica APE 4 · Prototipado – Wireframes

Esta exposición es la **Fase 1 del APE 4**. Aquí se muestra cómo cada parte de la guía oficial (UTA · FISEI · Software · Interacción Humano/Computador, ciclo julio–diciembre 2026) se cumple con los productos del repositorio.

**Tema de la exposición:** Prototipos y wireframes · APE 4 – Fase 1/2
**Objetivo de la exposición:** construir la Fase 1 del APE 4 y enseñar a la clase cómo se pasa de requisitos a arquitectura, flujo y wireframe.
**Entregable pedido:** sitemap + user flow + wireframes iniciales + explicación didáctica del proceso.

## 1. Objetivo de la guía → Fase 1
| La guía pide | Cómo lo cumple la Fase 1 |
|---|---|
| Objetivo: «Crear un prototipo usable aplicando un wireframe» | La Fase 1 construye la base del prototipo: lo que se debe definir **antes** de poder hacer clic en algo. Wireframes de la Tarea 1 en `prototipos/06-wireframes/lofi/`. |
| Resultado: «Formación de un desarrollador que pueda lograr una vista o idea de su proyecto de manera fácil» | El proceso requisitos → sitemap → navegación → user flow → componentes → wireframe → trazabilidad se puede repetir con cualquier proyecto (`prototipos/plantilla-en-blanco.md`). |

## 2. Pasos de la guía → productos del repositorio
| Paso de la guía | Dónde se cumple |
|---|---|
| 1. Revisar el material sobre wireframes en la creación de prototipos | `docs/investigacion.md` (Parte 1: conceptos) y las diapositivas en `src/fuentes-diagramas/` |
| 2. Generar un prototipo aplicando elementos usables de interacción | Componentes con estados (`prototipos/05-componentes.md`) colocados en los wireframes Lo-Fi, y adelanto Mid-Fi / Hi-Fi (`prototipos/06-wireframes/midfi`, `hifi`) |
| 3. Aplicar los criterios de un buen diseño | Heurísticas de Nielsen H1, H3, H4 y H5 en navegación y componentes; decisiones D1–D7 con su alternativa en `docs/decisiones.md` |
| 4. Elaborar las conclusiones | `docs/conclusiones.md` (individuales y del grupo) |
| 5. Subir el archivo a la plataforma en la fecha indicada | Se sube desde este repositorio (README y carpetas); ver «Entrega» abajo |

## 3. Fase 1 y Fase 2: cómo se entrelazan
| | Fase 1 (esta exposición) | Fase 2 (siguiente) |
|---|---|---|
| Pregunta | ¿Qué pantallas hay, cómo se recorren y qué contiene cada una? | ¿Se puede probar, hacer clic y navegar? |
| Productos | Requisitos, sitemap, navegación, user flow, componentes, wireframes Lo-Fi, trazabilidad | Prototipo navegable (pantallas enlazadas) a partir de los wireframes |
| Insumos | Historias de usuario HU-01, HU-02, HU-10, HU-11 | Todo lo de la Fase 1 |
| Ya adelantado en el repo | — | Mid-Fi y Hi-Fi de los mismos 4 cuadros |

Lo que la Fase 2 necesita de la Fase 1, y dónde está:
- **Qué pantallas enlazar:** sitemap (`02-sitemap.png`).
- **Qué elemento dispara cada salto:** tabla de navegación (`03-navegacion.md`).
- **En qué orden y con qué errores:** user flow (`04-user-flow.png`).
- **Qué piezas y estados dibujar y animar:** componentes (`05-componentes.md`).
- **Qué ve el usuario en cada momento:** wireframes (`06-wireframes/`).
- **Garantía de que no falta nada:** trazabilidad (`07-trazabilidad.md`).

## 4. Habilidades blandas de la guía
| Habilidad | Evidencia |
|---|---|
| Liderazgo | Cada integrante lidera un bloque y lo defiende (`docs/bloque-1-martin.md`, `bloque-2-david.md`, `bloque-3-sheyla.md`) |
| Trabajo en equipo | Ramas por tarea, Pull Requests con revisión cruzada (`.github/PULL_REQUEST_TEMPLATE.md`), `CONTRIBUCIONES.md` |
| Responsabilidad | Bitácoras con fechas reales (`evidencias/`) y entregas con issues y criterios de aceptación |

## 5. Bibliografía de la guía usada como marco
- Cañas, Granollers y Lorés (2012). *Diseño de sistemas interactivos centrados en el usuario.* UOC.
- Shneiderman, B. (2006). *Diseño de interfaces de usuario* (4.ª ed.). Pearson.
- Pressman, R. S. (2010). *Ingeniería del software* (7.ª ed.). McGraw-Hill. (modelamiento de sistemas)
- Córcoles y Montero (2015). *Diseño de interfaces web.* RA-MA.
- Pintos, J. (2024). *Aplicación de técnicas de usabilidad y accesibilidad en el entorno cliente.* Tutor Formación.

Las heurísticas de Nielsen citadas (H1, H3, H4, H5) corresponden a su conjunto de 10 heurísticas de usabilidad.

## 6. Entrega
Guía del APE 4 y entrega: se sube a la plataforma (aula virtual) **en la fecha indicada por el docente**; la fecha no figura en la guía, por lo que debe confirmarse en el aula virtual.
