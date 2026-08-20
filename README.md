# Guía PAP — Diseño de Modas · IDC 2026

Aplicación web interactiva y generador de documentos oficiales para el **Proyecto de Aplicación Profesional (PAP)** del Programa de Estudios de Diseño de Modas del **Instituto de Educación Superior Público Diseño y Comunicación (IDC)**, Lima, Perú.

---

## Descripción

Esta herramienta centraliza toda la información normativa, estructural y metodológica que los estudiantes necesitan para elaborar su PAP. Incluye un **formulario oficial validado** que genera automáticamente el documento Word del Plan del PAP con formato APA 7.ª edición, listo para presentar a la Coordinación del Programa de Estudios de Diseño de Modas.

---

## Características principales

- **Marco normativo integrado** — Referencias a Ley N.° 30512, D.S. N.° 010-2017-MINEDU, RVM N.° 103-2022-MINEDU, Lineamientos Académicos Generales para los IES, Normas APA 7.ª ed. y Memorando Múltiple N.° 05-JUI-IDC-2025-II.
- **6 líneas transversales institucionales** — Sostenibilidad ambiental, Transformación digital, Identidad cultural, Emprendimiento, Educación y cambio social, e Inclusión y accesibilidad.
- **5 fichas de investigación** para el Programa de Estudios de Diseño de Modas:
  - `DM-L1` Moda sostenible y reciclaje textil
  - `DM-L2` Innovación textil
  - `DM-L3` Diseño de moda inclusivo
  - `DM-L4` Tendencias y consumo responsable
  - `DM-L5` Tecnología en la moda
- **Verbos de Bloom** — Tabla interactiva clasificada por nivel cognitivo (Conocimiento → Síntesis), con advertencia automática si se detectan verbos en tiempo pasado en los objetivos.
- **Comparativa Plan vs. Informe** — Diferencias clave entre ambos documentos con gráficos Chart.js interactivos: distribución de esfuerzo por capítulo (doughnut) y radar de calidad PAP estándar vs. PAP de excelencia.
- **Especificaciones de formato APA 7** — Parámetros institucionales inamovibles: Times New Roman 12 pt, interlineado 1.5, márgenes, numeración y jerarquía de encabezados (Niveles 1–5).
- **Apéndices recomendados** — Tarjetas flip 3D (A–J); A, B y C son obligatorios en el Informe final.
- **Generador de documentos Word** — Formulario de 10 secciones con validación en tiempo real que exporta un archivo `.docx` con estructura institucional y portada oficial.
- **Guardado de borrador automático** — Los datos del formulario se guardan en `localStorage` y se restauran al recargar la página.
- **Modo PWA** — Instalable como aplicación web progresiva en dispositivos móviles y de escritorio.

---

## Estructura del proyecto

```
/
├── index.html          # Aplicación completa (single-file HTML)
├── LogoIDC.png         # Logotipo institucional del IDC
└── README.md           # Documentación del proyecto
```

> Toda la lógica (HTML, CSS, JavaScript, generación de Word y compresión ZIP) está embebida en `index.html`. No requiere servidor backend ni dependencias npm; solo un navegador moderno.

---

## Dependencias externas (CDN)

| Librería | Uso |
|---|---|
| Bootstrap 5.x | Sistema de rejilla y componentes UI |
| Chart.js 4.x | Gráficos doughnut y radar |
| JSZip (implementación nativa interna) | Generación del archivo `.docx` en cliente sin servidor |

---

## Líneas de investigación — Diseño de Modas

Cada línea incluye: objetivo general modelo, objetivos específicos modelo (OE1–OE3), tabla de elementos técnicos y conceptuales, tipos y categorías, y tabla de metodología por fases.

| Código | Línea | Subsector |
|---|---|---|
| DM-L1 | Moda sostenible y reciclaje textil | Industria textil, emprendimientos de moda sostenible, comercio justo |
| DM-L2 | Innovación textil | Manufactura de confecciones de exportación, moda técnica y deportiva |
| DM-L3 | Diseño de moda inclusivo | Moda adaptada para PCD, plus size, gerontomoda |
| DM-L4 | Tendencias y consumo responsable | Consultoría de moda, bureaux de tendencias, marcas de moda |
| DM-L5 | Tecnología en la moda | Fashion tech, e-commerce, plataformas de moda digital, metaverso |

---

## Formulario: secciones del Plan PAP

El formulario oficial cubre las 10 secciones institucionales:

| N.° | Sección | Descripción |
|---|---|---|
| 1 | Título del trabajo | Máx. 25 palabras: verbo de acción + objeto + línea temática + lugar + año |
| 2 | Programa de estudios | Carrera fija (Diseño de Modas), año de egreso, línea DM y línea transversal |
| 3 | Integrantes | Matrícula, nombres, teléfono, correo (máx. 2 del mismo programa; 4 si es multidisciplinario) + Asesor |
| 4 | Formulación del problema | Problema general (pregunta central) y problemas específicos |
| 5 | Objetivos | Objetivo general y específicos con verbos en infinitivo prospectivo |
| 6 | Justificación | Trascendencia, magnitud, vulnerabilidad y factibilidad |
| 7 | Descripción técnica | Contenido y resultados esperados (máx. 300 palabras) |
| 8 | Cronograma | Resumen por fases; el Diagrama de Gantt completo va como Apéndice A |
| 9 | Presupuesto y recursos | Aportes financieros, laboratorios, equipos y materiales |
| 10 | Referencias bibliográficas | APA 7.ª ed., orden alfabético, antigüedad máx. 5 años |

---

## Uso

1. **Abrir** `index.html` directamente en el navegador (sin servidor requerido).
2. **Navegar** por las secciones informativas para familiarizarse con la normativa y las líneas de investigación DM.
3. **Completar** el formulario en la sección *Generador del Plan* (sección 12).
   - Usar **Cargar datos de DEMO** para previsualizar un ejemplo completo de moda sostenible.
   - Usar **Solo la Plantilla en blanco** para descargar la plantilla vacía en Word.
4. **Generar** el documento: presionar **Generar documento en Word**. El archivo `.docx` se descarga con nombre `PlanPAP_DM-LX_<ApellidoEstudiante>.docx`.
5. **Instalar** como PWA (botón flotante inferior derecho) para acceso sin conexión.
6. Los datos del formulario se **guardan automáticamente** en el navegador como borrador al escribir y se restauran al recargar la página.

---

## Autoridades institucionales

| Cargo | Nombre |
|---|---|
| Coordinación del Programa de Estudios de Diseño de Modas | Mg. Fany Picón Tejedo |
| Jefatura de la Unidad de Investigación | Mg. Mario Quiroz Martínez |

---

## Marco normativo aplicado

- **Ley N.° 30512** — Ley de Institutos y Escuelas de Educación Superior (Art. 21: investigación aplicada e innovación como modalidad de titulación).
- **D.S. N.° 010-2017-MINEDU** — Reglamento de la Ley N.° 30512 y sus modificatorias.
- **Resolución Viceministerial N.° 103-2022-MINEDU** — Condiciones Básicas de Calidad (CBC) para IES Tecnológicos.
- **Lineamientos Académicos Generales para los IES** — Organización curricular, perfiles de egreso y titulación.
- **Normas APA, 7.ª edición** — Citación y referencias bibliográficas en todo el informe.
- **Memorando Múltiple N.° 05-JUI-IDC-2025-II** — Aprobación de las veinte líneas de investigación institucionales.

---

## Compatibilidad

Probado en Chrome 120+, Firefox 121+, Edge 120+ y Safari 17+. Se recomienda pantalla de al menos 768 px de ancho para una experiencia óptima del formulario.

---

## Licencia

© 2026 Instituto de Educación Superior Público Diseño y Comunicación — Lima, Perú. Todos los derechos reservados.  
Uso exclusivo para fines académicos e institucionales del IDC.
