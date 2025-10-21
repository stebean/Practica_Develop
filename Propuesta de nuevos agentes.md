# Propuesta de nuevos agentes (MVP y Post‑MVP)

Autor: Esteban de Santiago García

Fecha: 2025-10-21

Contexto
- Basado en: mvp.md, prd.md
- Agentes existentes: Product Owner, Analista de Software, Arquitecto de Software, Generador de Agentes
- Objetivo: Proponer agentes adicionales que maximicen valor, claridad y calidad del MVP (app pública, lectura de agentes/equipos)

Leyenda de importancia
- Crítico: indispensable para cumplir el MVP con calidad
- Alto: aporta valor claro en el MVP
- Medio: útil pero puede esperar si hay presión de tiempo
- Bajo: enfocado a Post‑MVP

Agentes propuestos para el MVP

1) Agente de Calidad y Pruebas (QA/Test Agent)
- Objetivo: Asegurar que lo entregado cumple criterios de aceptación, estados de UX y DoD.
- Responsabilidades:
  - Convertir criterios de aceptación en casos de prueba (happy/edge cases).
  - Diseñar pruebas de navegación (listas/detalles) y estados (cargando/vacío/error).
  - Preparar plan de prueba para demo y checklist de regresión por Sprint.
- Entregables: Matriz HU↔CA↔Pruebas, checklist DoD, reporte de resultados de pruebas.
- Interacciones: Analista (CA), Arquitecto (errores estándar), PO (aceptación).
- Importancia: Crítico (MVP).

2) Agente de Curación de Datos (Data Curation Agent)
- Objetivo: Garantizar datos de ejemplo coherentes y suficientes para una experiencia fluida.
- Responsabilidades:
  - Preparar semillas mínimas (≥3 equipos, ≥5 agentes, ≥6 miembros).
  - Verificar enlaces specUrl/repoUrl y consistencia de nombres/roles.
  - Mantener un data dictionary no técnico (términos, convenciones).
- Entregables: Dataset semilla, guía de nomenclatura, checklist de consistencia de datos.
- Interacciones: Analista (glosario), Arquitecto (modelo de datos), PO (relevancia de contenido).
- Importancia: Alto (MVP).

3) Agente de UX de Contenido (UX Content Agent)
- Objetivo: Alinear mensajes, microcopy y jerarquía de información con una experiencia clara.
- Responsabilidades:
  - Definir textos para vacíos/errores/llamados a acción.
  - Estandarizar cómo se presenta cada agente/equipo (resumen corto, chips de capacidades).
  - Revisar consistencia de etiquetas y navegación.
- Entregables: Guía de contenidos (microcopy), pautas de tarjetas/listas/detalles.
- Interacciones: Analista (flujos y estados), PO (tono), Arquitecto (limitaciones técnicas).
- Importancia: Alto (MVP).

4) Agente de Entrega y Release (Release Agent)
- Objetivo: Coordinar entregables visibles por Sprint y la preparación de la demo.
- Responsabilidades:
  - Definir criterios de “listo para demo” y notas de versión.
  - Orquestar checklist previo a demo (datos, endpoints, estados, métricas básicas).
  - Alinear calendario de hitos y responsables.
- Entregables: Plan de release del MVP, notas de versión por Sprint, checklist pre‑demo.
- Interacciones: PO (prioridades y alcance), Arquitecto (riesgos técnicos), QA (resultados).
- Importancia: Alto (MVP).

5) Agente de Observabilidad Ligera (Observability Agent)
- Objetivo: Asegurar que los errores y eventos clave se puedan entender en demo y pruebas.
- Responsabilidades:
  - Definir taxonomía de errores {code, message} y ejemplos.
  - Acordar eventos mínimos a registrar (cargas de listas/detalles, fallos).
  - Consolidar un formato de reporte breve para issues encontrados.
- Entregables: Guía de errores y eventos, ejemplo de reporte de incidentes.
- Interacciones: Arquitecto (NFRs), QA (hallazgos), PO (impacto en demo).
- Importancia: Medio (MVP).

6) Agente de Accesibilidad Básica (A11y Agent)
- Objetivo: Mejorar legibilidad y uso básico para todos los usuarios.
- Responsabilidades:
  - Revisar contraste, tamaños de texto y foco en navegación esencial.
  - Recomendar ajustes simples sin impacto técnico mayor.
- Entregables: Checklist a11y básica y recomendaciones aplicables al MVP.
- Interacciones: Analista/UX (mensajes), PO (prioridad de cambios menores).
- Importancia: Medio (MVP).

Agentes propuestos Post‑MVP

7) Agente de Contenido Multimedia (Media Agent)
- Objetivo: Diseñar cómo incorporar grabaciones/sesiones de forma usable y ligera.
- Responsabilidades: Directrices de formatos, enlaces, metadatos y políticas de visibilidad.
- Entregables: Guía de integración de media y flujo de publicación.
- Importancia: Bajo (Post‑MVP).

8) Agente de Autenticación y Acceso (Auth Agent)
- Objetivo: Planificar un acceso básico cuando el producto lo requiera.
- Responsabilidades: Definir escenarios de login, perfiles y permisos futuros.
- Entregables: Mapa de roles/permiso y flujos de autenticación.
- Importancia: Bajo (Post‑MVP).

9) Agente de Rendimiento y Escalabilidad (Performance Agent)
- Objetivo: Preparar el camino para más datos/usuarios.
- Responsabilidades: Recomendaciones de consultas, caché y pruebas de carga.
- Entregables: Plan de performance básico y métricas objetivo Post‑MVP.
- Importancia: Bajo (Post‑MVP).

10) Agente de Seguridad y Privacidad (Security/Privacy Agent)
- Objetivo: Elevar controles básicos a un nivel formal cuando crezca el alcance.
- Responsabilidades: Revisión de PII, encabezados, políticas de CORS y buenas prácticas.
- Entregables: Checklist de seguridad y plan de mejoras.
- Importancia: Medio (Post‑MVP).

Resumen de importancia (MVP)
- Crítico: QA/Test
- Alto: Curación de Datos, UX de Contenido, Entrega/Release
- Medio: Observabilidad Ligera, Accesibilidad Básica
- Bajo: (N/A en MVP)

Notas finales
- Cada agente colabora con PO, Analista y Arquitecto respetando límites: el PO define el “qué y por qué”; los agentes propuestos facilitan “cómo logramos calidad y claridad” sin imponer tecnología.
- Si hay presión de tiempo, activar primero QA/Test y Curación de Datos para asegurar una demo sólida.
