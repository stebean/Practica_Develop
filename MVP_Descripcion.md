# MVP Definition: Project Showcase App

## 1. Product Goal

El objetivo de este producto es crear una aplicación pública para mostrar de forma transparente y atractiva el trabajo y los resultados del proyecto, centrada en los agentes desarrollados y los equipos que los crearon.

## 2. High-Level Vision

Queremos una aplicación intuitiva y visualmente agradable donde cualquier persona pueda explorar los agentes de IA que se han construido, entender su propósito y conocer a los equipos y desarrolladores detrás de ellos.

---

## 3. MVP: Core Features

Para la primera versión (MVP), nos centraremos en entregar el valor fundamental, que es mostrar los resultados tangibles del proyecto.

### Epic 1: Visualización de Agentes
Como usuario, quiero poder ver todos los agentes que se crearon para entender el alcance del trabajo realizado.

*   **Feature:** Pantalla principal con una lista/galería de todos los agentes.
*   **Feature:** Al seleccionar un agente, puedo ver toda su información (descripción, rol, capacidades, etc., extraído de su archivo de especificación).

### Epic 2: Visualización de Equipos y Desarrolladores
Como usuario, quiero conocer a las personas que construyeron estos agentes.

*   **Feature:** Pantalla con la lista de equipos que participaron en el proyecto.
*   **Feature:** Al seleccionar un equipo, puedo ver los miembros que lo conformaron.
*   **Feature:** Desde la vista de un agente, puedo navegar para ver la información de su desarrollador principal (nombre, rol desempeñado).

---

## 4. Technology Stack (Confirmado para el MVP)

*   **Frontend:** Flutter
*   **Backend:** Java con Spring Boot
*   **Base de Datos / BaaS:** Supabase (para una rápida integración inicial con Flutter)
*   **Comunicación:** API REST para conectar el frontend de Flutter con el backend de Java.

---

## 5. Out of Scope for the MVP

Para asegurar una entrega rápida y enfocada, las siguientes funcionalidades se considerarán para futuras versiones:

*   **Métricas de Desempeño Individual:** No se mostrará información detallada sobre el desempeño, asistencia o avances de cada desarrollador. Esto requiere más análisis sobre la privacidad y la objetividad de los datos.
*   **Grabaciones de Sesiones:** La visualización de videos no se incluirá en esta primera versión.
*   **Explorador de Carpetas:** No se mostrará la estructura de carpetas cruda de los integrantes.
*   **Autenticación de Usuarios:** La aplicación será pública y no requerirá login.
