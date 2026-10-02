# Plan del Trabajo de Aplicación Profesional (TAP) — Diseño de Modas · IDC 2026

Aplicación web interactiva y **generador de documentos oficiales** para el **Trabajo de Aplicación Profesional (TAP)** del Programa de Estudios de Diseño de Modas del **Instituto de Educación Superior Público «Diseño y Comunicación» (IDC)**, Lima, Perú.

Sitio publicado: <https://uinvestigacion-idc.github.io/JUI_TAP_DisModas/>

---

## Descripción general

`index.html` es una aplicación **single-file** (HTML + CSS + JavaScript embebidos, sin backend ni dependencias npm) que:

1. **Ordena la información normativa, metodológica y de líneas de investigación** del TAP conforme al *Manual para el desarrollo del Trabajo de Aplicación Profesional (TAP) — Diseño de Modas* (IDC, 2026).
2. **Guía el llenado del Plan del TAP** con un formulario oficial validado y **ayuda contextual mediante cuadros de diálogo emergentes**.
3. **Genera el documento Word** (`.docx`) del Plan, con portada institucional, formato APA 7.ª edición y declaración de uso de IA cuando corresponde.

> **Naturaleza del documento generado.** El generador produce un **informe preliminar** —un borrador estructurado del Plan— y **no** la versión definitiva del TAP. Descargar el archivo no equivale a haber concluido el Plan: se requiere (1) la confirmación de la Coordinación Académica, y (2) la ampliación y aprobación del docente asesor.

---

## Novedades de esta versión (migración PAP → TAP)

| Antes (versión PAP) | Ahora (versión TAP) |
|---|---|
| «Plan del Proyecto de Aplicación Profesional (PAP)» | **«Plan del Trabajo de Aplicación Profesional (TAP)»** en título, encabezado, hero, formulario, pie, PWA y documento Word |
| 6 instrumentos normativos | **8 instrumentos**, incluido el Reglamento de uso de IA en trabajos académicos del IDC (2026), arts. 9 y 18-A |
| 10 secciones del Plan | **8 apartados (1.1 a 1.8)** conforme a la Parte I del manual |
| Solo 5 líneas DM | **5 líneas DM (referente temático) + 4 líneas del TAP (A, B, C, D)** con módulos de desempeño, matriz de módulos formativos y tabla de correspondencia |
| Sin sección de IA | **Parte IV completa**: marco AIAS (5 niveles), límite autoral, uso permitido/no permitido por fase, declaración, citación APA 7 de IA, alucinaciones y bitácora de prompts |
| Verbos «Conocimiento → Síntesis» | **«Recordar, Comprender, Aplicar, Analizar, Crear»** con su uso en Diseño de Modas |
| Plan vs. Informe (comparativa simple) | **Partes II y III**: 12 secciones 8.1–8.12, claves por sección, tipos de investigación, metodologías por línea y mapa de extensiones |
| Sin checklist | **Parte VII**: checklist interactivo de Plan, Informe Final y exposición con jurado, minuto a minuto (20:00) y «qué no va en pantalla» |
| Sin requisitos de sustentación | **Parte VIII**: requisitos académicos, documentales, de recursos y lista de verificación previa |
| Ayuda en texto plano (`form-help-tip`) | **24 temas de ayuda en cuadros de diálogo emergentes** + índice general + botón flotante «Guía del formulario» |
| Sin campos de IA | Campos de **uso de IA, nivel AIAS, aprobador, herramientas, fases, finalidad y bitácora de prompts** |

---

## Características principales

### Contenido normativo y metodológico
- **Orientación preliminar** con las tres etapas del flujo institucional de aprobación y la regla operativa del borrador.
- **Marco normativo** (Ley N.° 30512, D.S. N.° 010-2017-MINEDU, RVM N.° 103-2022-MINEDU, Lineamientos Académicos Generales para los IES, APA 7.ª ed., Memorando Múltiple N.° 05/JUI/IDC/2025-II, Reglamento IA IDC 2026 y Reglamento del Estudiante).
- **Líneas transversales institucionales** (6 ejes) con adscripción obligatoria a una o más.
- **Líneas del TAP A–D** con sus módulos de desempeño y módulo formativo asociado, más la **matriz de relación** y la **correspondencia DM → TAP**.
- **Cinco fichas DM** (L1–L5) con sector, producto, materiales/innovaciones/adaptaciones, técnicas, entregables, validación y línea del TAP sugerida.
- **Del Plan al Informe Final**: estructura de 12 secciones (8.1–8.12), claves de contenido y extensión por sección, tipos de investigación (aplicada, I+D, innovación tecnológica), metodologías sugeridas por línea y mapa de extensiones.
- **IA generativa**: condiciones no negociables (transparencia, autoría humana, verificación), marco AIAS, límite autoral en Diseño de Modas, usos permitidos y no permitidos por fase, declaración general y específica, citación APA 7, verificación de alucinaciones y bitácora de prompts.
- **Metodología y APA 7**: métodos hipotético-deductivo, inductivo y análisis-síntesis; citas parentéticas y narrativas; parámetros inamovibles de formato y jerarquía de encabezados (niveles 1–5).
- **Apéndices A–J** en tarjetas flip: A, B y C obligatorios; D, E, F, G, I recomendados; H «si aplica»; J opcional.

### Ayuda contextual por cuadros de diálogo emergentes
- **24 temas** de ayuda: título, programa e integrantes, líneas (DM, TAP, transversales), módulos de desempeño, módulo formativo, asesor, problema, objetivos, justificación y sus cuatro criterios, descripción técnica, cronograma, presupuesto, referencias, uso de IA, AIAS y bitácora.
- Cada cuadro reproduce **qué debe contener, ejemplos del manual, reglas y límites, y checklist** del apartado.
- **27 botones `?`** distribuidos en los apartados y campos del formulario, más un botón **«Guía rápida del formulario»** y un botón flotante **«Guía del formulario»** que abre el índice temático.
- Navegación interna **«← Anterior / Índice de ayuda / Entendido»**, cierre con `Esc`, clic en el fondo o botón, **foco accesible** y contención de tabulación.

### Formulario oficial del Plan del TAP
14 bloques con validación en tiempo real:

| N.° | Bloque | Contenido |
|---|---|---|
| 1 | Título del trabajo | Máx. 25 palabras; contador en vivo; verbo + objeto + línea + lugar + año |
| 2 | Programa de estudios | Carrera bloqueada («Diseño de Modas»), semestre/año de egreso, año de presentación |
| 3 | Líneas de investigación | Línea DM, **línea del TAP (A–D)**, módulos de desempeño (dinámicos), módulo formativo y líneas transversales (casillas múltiples) |
| 4 | Integrantes | Dinámicos (hasta 4): matrícula, nombres, teléfono, correo y foto opcional |
| 5 | Asesor del proyecto | Docente del programa o especialista validado por la Coordinación |
| 6 | Formulación del problema | Problema general + problemas específicos |
| 7 | Objetivos | Objetivo general + específicos, con detección de verbos en pasado |
| 8 | Justificación | Trascendencia, magnitud, vulnerabilidad y factibilidad |
| 9 | Descripción técnica | Máx. 300 palabras con contador |
| 10 | Cronograma | Fases del proyecto (Apéndice A: Gantt) |
| 11 | Presupuesto, medios y materiales | Categorías con contingencias del 10 % (Apéndice B) |
| 12 | Referencias bibliográficas | APA 7.ª ed., mínimo 5 en el Plan |
| 13 | Uso de IA generativa (AIAS) | ¿Se usó IA?, nivel AIAS, aprobador, herramientas, fases y finalidad |
| 14 | Bitácora de prompts | Una interacción por línea para el apéndice del Informe Final |

**Validaciones implementadas:** campos obligatorios con lista de faltantes, al menos una línea transversal, al menos un módulo de desempeño cuando la línea es A, B o C, advertencia de verbos en pasado, límites de 25/300 palabras y mínimo de integrantes.

### Checklist de validación interactivo (Parte VII)
- **53 ítems** con casillas: 14 del Plan del TAP, 16 del Informe Final, 15 de la exposición con jurado y 8 de la lista previa a la sustentación.
- Barras de avance y contador por bloque; estado **«✔ Completo»** al terminar.
- **Persistencia en `localStorage`** (clave `idc_tap_checklist_v1`), independiente del borrador del formulario.
- Incluye el **minuto a minuto (20:00)** de la exposición, «Qué no va en pantalla», el ensayo y la regla de oro.

### Generador de documentos Word
- Genera un `.docx` real **en el navegador** (ZIP `STORE` propio con CRC-32, sin librerías externas ni servidor).
- Contenido del documento: portada institucional TAP, título, programa/líneas/módulos, tabla de autores, asesor y lugar-año; **Declaración de uso de IA** (tras la portada, cuando se declara uso de IA); nota institucional de informe preliminar; apartados **1.1 a 1.8**; apéndice de **bitácora de prompts**; firmas con DNI.
- Formato institucional: Times New Roman 12, interlineado 1.5, texto justificado, sangría de primera línea, márgenes APA (izquierdo 1985 twips ≈ 35 mm), encabezado y pie con numeración de página.
- Nombres de archivo:
  - `Plan_TAP_<LíneaTAP>_<PrimerApellido>.docx`
  - `Plan_TAP_Diseno_Modas_PLANTILLA_2026.docx` (plantilla en blanco)

### Otras funciones
- **Carga de datos DEMO** con un caso completo de moda sostenible (DM-L1 → línea B, Módulo II, con IA declarada en nivel 3).
- **Autoguardado de borrador** en `localStorage` (clave `idc_tap_dm_borrador_v1`) con restauración al recargar, incluidos los módulos de desempeño y las líneas transversales.
- **Botón Limpiar formulario** que reinicia campos, integrantes, módulos, transversales y borrador.
- **Gráficos Chart.js**: distribución de hojas por sección del Informe Final (doughnut) e indicadores de calidad TAP estándar vs. de excelencia (radar).
- **PWA instalable** con manifest e *service worker* generados en tiempo de ejecución (iconos `TAP`).

---

## Estructura del proyecto

```
JUI_TAP_DisModas/
├── index.html                              # Aplicación completa (single-file HTML/CSS/JS)
├── README.md                               # Este documento
├── Logo_IDC.png                            # Logotipo institucional (encabezado, pie y formulario)
├── Logo_IDC - copia.jpg                     # Logotipo alterno (encabezado)
├── Manual_TAP_Disenio_Modas_IDC2026.md      # Manual del TAP en Markdown
├── Manual_TAP_Disenio_Modas_IDC2026.docx    # Manual del TAP en Word
├── Manual_TAP_Disenio_Modas_IDC2026.pdf     # Manual del TAP en PDF
└── Archivos/                                # Materiales de versiones previas (PAP)
    ├── README.md                            # README de la versión PAP (histórico)
    ├── index22.html                         # Versión anterior del index
    └── Manual_PAP_*.{md,docx,pdf,…}         # Manuales PAP previos
```

> Toda la lógica (interfaz, ayuda contextual, validaciones, checklist, generación de Word y compresión ZIP) está embebida en `index.html`. No requiere servidor backend, instalación ni compilación: basta un navegador moderno.

---

## Mapa de contenido de la página

| N.° | Sección | Parte del manual |
|---|---|---|
| 01 | Presentación institucional y naturaleza del documento generado | Orientación preliminar |
| 02 | Marco normativo (8 instrumentos) | — |
| 03 | Líneas transversales institucionales | 1.3 |
| 04 | Líneas de investigación del TAP (A–D), módulos y matriz | 5.6 – 5.8 |
| 05 | Cómo llenar el formulario del Plan del TAP (1.1 – 1.8) | Parte I |
| 06 | Taxonomía de objetivos (verbos de Bloom) | 1.5 |
| 07 | Justificación del proyecto (4 criterios) | 1.6 |
| 08 | Del Plan al Informe Final (8.1 – 8.12, tipos y metodologías, extensiones) | Partes II y III |
| 09 | Líneas DM del programa (fichas L1–L5) | Parte V |
| 10 | Uso e implementación de la IA generativa en el TAP | Parte IV |
| 11 | Metodología, citas y formato APA 7 | Parte VI |
| 12 | Apéndices obligatorios y recomendados (A–J) | 6.5 |
| 13 | Checklist de validación antes de la entrega | Parte VII |
| 14 | Requisitos para la sustentación del TAP | Parte VIII |
| 15 | Generador del Plan del TAP (formulario + ayuda) | Parte I |

---

## Líneas del TAP y módulos de desempeño

| Línea | Denominación | Módulos de desempeño | Módulo formativo |
|---|---|---|---|
| **A** | Desarrollo de producto y producción textil | 7 módulos (colecciones, fichas técnicas, patronaje y tizado, muestras y prototipos UDP, fitting y control de calidad, compras de insumos, confección y costos) | Módulo I y Módulo III |
| **B** | Innovación y experimentación aplicada | 5 módulos (moda digital, simulación 3D, biomateriales, upcycling, fashion tech y wearables) | Módulo II |
| **C** | Gestión, comunicación y comercialización de moda | 11 módulos (compras internacionales, stock, e-commerce, catálogos, branding, marketing, visual merchandising, styling, audiovisual, contenido digital, coolhunting) | Módulo I y III (énfasis en gestión) |
| **D** | Proyectos interdisciplinarios o especiales | 3 módulos (integración de áreas, disciplinas afines, alcance especial) | Según alcance aprobado por la Coordinación |

**Correspondencia DM → TAP (orientativa):** DM-L1 → B (con producto de A) · DM-L2 → A y B · DM-L3 → A · DM-L4 → C · DM-L5 → B.

---

## Uso

1. **Abrir** `index.html` en el navegador o ingresar al sitio publicado (no requiere servidor).
2. **Recorrer** las secciones 01–14 para conocer la normativa, las líneas y los checklists.
3. **Completar** el formulario en la sección 15 (*Generador del Plan del TAP*):
   - Pulsar los botones **`?`** de cada apartado para abrir los **cuadros de diálogo de ayuda**; el botón flotante **«Guía del formulario»** abre el índice temático.
   - Declarar la **línea del TAP** para que aparezcan los **módulos de desempeño** correspondientes.
   - Marcar **una o más líneas transversales**.
   - Si se usó IA generativa, declarar el **nivel AIAS** y completar herramientas, fases, finalidad y la **bitácora de prompts**.
   - Usar **Cargar datos de DEMO** para previsualizar un ejemplo completo o **Solo la Plantilla (en blanco)** para descargar la plantilla vacía.
4. **Generar** el documento con **Generar documento en Word**; el `.docx` se descarga automáticamente.
5. **Verificar** el Plan con el **checklist interactivo** (sección 13) antes de enviarlo.
6. **Instalar** como PWA desde el botón flotante inferior derecho para uso sin conexión.

### Restablecer datos guardados
- Borrador del formulario: `localStorage.removeItem('idc_tap_dm_borrador_v1')`
- Checklist: `localStorage.removeItem('idc_tap_checklist_v1')`
- O usar el botón **Limpiar formulario** para el borrador.

---

## Dependencias externas (CDN)

| Librería | Uso |
|---|---|
| Bootstrap 5.3.3 (CSS y JS) | Rejilla y utilidades de interfaz |
| Chart.js 4.4.4 | Gráficos doughnut y radar |
| Google Fonts (Bricolage Grotesque, Manrope, JetBrains Mono) | Tipografía institucional |

La generación del `.docx` **no** usa librerías externas: se implementa con un empaquetador ZIP propio (`makeZip`) y CRC-32 en JavaScript.

---

## Notas de mantenimiento

| Qué editar | Dónde (en `index.html`) |
|---|---|
| Textos de la ayuda contextual | Objeto `HELP` (24 temas con `code`, `t`, `s`, `h`) |
| Módulos de desempeño por línea y sugerencia de módulo formativo | `MODULOS_TAP` y `MODULO_FORMATIVO_SUGERIDO` |
| Estructura del documento Word | Función `buildDocument(d)` (portada, apartados 1.1–1.8, apéndice de bitácora, firmas) |
| Datos del ejemplo | Función `cargarDemo()` |
| Plantilla en blanco | Función `buildPlantilla()` |
| Parámetros de formato APA (fuente, márgenes, interlineado) | `stylesXML`, `documentXML` y `w:sectPr` dentro de `buildDocument()` |
| Ítems del checklist | Bloques `.checklist-wrap` con atributos `data-cl` |
| Paleta y estilos | Variables CSS en `:root` y bloque `<style>` |
| Enlaces institucionales | Secciones 01 y 05 (recursos de apoyo del manual) |

**Recomendación:** cualquier cambio en los requisitos debe contrastarse con `Manual_TAP_Disenio_Modas_IDC2026.md` (o su versión PDF/DOCX) para mantener la trazabilidad con el manual.

---

## Marco normativo aplicado

- **Ley N.° 30512** — Ley de Institutos y Escuelas de Educación Superior (Art. 21: investigación aplicada e innovación como modalidad de titulación).
- **D.S. N.° 010-2017-MINEDU** — Reglamento de la Ley N.° 30512 y sus modificatorias.
- **Resolución Viceministerial N.° 103-2022-MINEDU** — Condiciones Básicas de Calidad (CBC) para los IES Tecnológicos.
- **Lineamientos Académicos Generales para los IES** — Organización curricular, perfiles de egreso y titulación.
- **Normas APA, 7.ª edición** (American Psychological Association, 2020) — Estándar único de citación y referenciación.
- **Memorando Múltiple N.° 05/JUI/IDC/2025-II** — Aprobación de las líneas de investigación institucionales y del catálogo de líneas del TAP.
- **Reglamento de uso de IA en trabajos académicos del IDC (2026)** — Arts. 9 y 18-A: declaración obligatoria, uso filtrado, verificación y revisión de originalidad.
- **Reglamento del Estudiante del IDC** — Consecuencias de la omisión o falsedad de la declaración de uso de IA.

---

## Autoridades institucionales

| Cargo | Nombre |
|---|---|
| Coordinación del Programa de Estudios de Diseño de Modas | Mg. Fany Picón Tejedo · modasjefatura@idc.edu.pe |
| Jefatura de la Unidad de Investigación | Mg. Mario Quiroz Martínez |

---

## Recursos institucionales

- Formulario TAP — Diseño de Modas: <https://uinvestigacion-idc.github.io/JUI_TAP_DisModas/>
- Bibliometría IDC: <https://uinvestigacion-idc.github.io/JUI_BiblioIA/>
- Guía institucional APA 7, IA generativa y declaración de uso: <https://uinvestigacion-idc.github.io/JUI_Decla_IA2026/>

---

## Verificaciones realizadas

- **JavaScript**: `node --check` sobre el script embebido, sin errores de sintaxis.
- **HTML**: balance de etiquetas verificado con analizador estructural, **0 errores**.
- **Referencias internas**: todas las llamadas `onclick` y todas las claves del objeto `HELP` resuelven; ningún `getElementById` apunta a un id inexistente.
- **Documento Word**: `.docx` generado y validado (ZIP íntegro, 12 tablas, todos los XML bien formados, textos clave presentes).

---

## Compatibilidad

Probado en Chrome 120+, Firefox 121+, Edge 120+ y Safari 17+. Se recomienda un ancho de pantalla de al menos 768 px para la experiencia óptima del formulario; los cuadros de diálogo de ayuda son adaptables a móvil.

---

## Publicación en GitHub Pages

1. Confirmar que `index.html` y `README.md` estén en la raíz de la rama publicada.
2. En el repositorio: **Settings → Pages → Source** (rama y carpeta raíz) y guardar.
3. Verificar el sitio en <https://uinvestigacion-idc.github.io/JUI_TAP_DisModas/>.

---

## Licencia

© 2026 Instituto de Educación Superior Público «Diseño y Comunicación» — Lima, Perú. Todos los derechos reservados.
Uso exclusivo para fines académicos e institucionales del IDC.
