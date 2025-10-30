# IDSW1-Proyecto final

##  Plataforma de Gestión de Proyectos de Investigación FUNIBER

## I. Contexto y Objetivos

El objetivo principal es desarrollar una **plataforma de gestión integral (tipo red profesional)** para el Departamento de Proyectos de Investigación de FUNIBER.

**Propósito Clave:**
* **Centralizar** perfiles académicos, convocatorias y proyectos.
* **Optimizar** la asignación de recursos y evitar la sobrecarga docente/investigadora.
* **Garantizar la trazabilidad** del ciclo completo del proyecto: de la propuesta a la compensación.


## II. Actores y Roles Clave

| Rol | Alcance y Responsabilidad Principal |
| :--- | :--- |
| **Investigador / Docente** | Gestión de su propio perfil, presentación de Propuestas (como **Antena**), ejecución de Proyectos y registro de Entregables. |
| **Personal Dpto. Proyectos (DP)** | Administración central, selección de la **Antena** idónea, supervisión del progreso y gestión de alertas. |
| **Directivos (Rector, VV.RR.)** | Consulta de Indicadores, estadísticas y rendimiento general de la investigación. |
| **Área de Finanzas** | Gestión de presupuestos, nóminas y registro de Compensaciones económicas o de reducción horaria. |
| **Colaborador** | Participa en proyectos, figura en la base de datos, pero **sin acceso** al sistema. |



## III. Modelo de Dominio (Entidades Esenciales)

| Entidad | Descripción Clave |
| :--- | :--- |
| **Persona / Perfil** | Datos personales, académicos (CV integrado, publicaciones), y rol (Investigador/Docente). |
| **Carga de Trabajo** | Horas semanales de docencia e investigación de una Persona. |
| **Convocatoria** | Oportunidad de financiación (SODERCAN, UE, etc.). |
| **Propuesta** | Documento o solicitud presentada. Registra estado (Aceptada/Rechazada) para el histórico. |
| **Proyecto** | Propuesta aceptada. Contiene responsables, importe, duración, objetivos y lista de Entregables. |
| **Entregable** | Hito o producto comprometido (ej. informes) con su fecha límite (**deadline**). |
| **Compensación** | Retribución final (económica o reducción horaria) por la participación en un Proyecto. |
| **RolProyecto** | Define la función específica de una Persona dentro de un Proyecto (Principal, Asociado, Colaborador, Finanzas). |



## IV. Reglas de Negocio Críticas

El sistema debe validar y aplicar las siguientes reglas sin excepción:

1.  **Límite de Carga Docente:** El Investigador-Docente tiene un **máximo de 16 horas/semana (4 asignaturas)**. El sistema **no debe permitir** la asignación de un proyecto (como Antena) si esta carga se supera.
2.  **Compensación de Docentes:** Al finalizar un Proyecto, el Investigador-Docente **debe elegir** entre:
    * Compensación económica.
    * **Reducción de horas docentes** futuras.
3.  **Trazabilidad:** Toda Propuesta (aceptada o rechazada) debe quedar registrada en el histórico.



## V. Casos de Uso Clave (Funcionalidades)

* **Gestión de Perfil:** Permitir la actualización del CV y la visualización de la Carga de Trabajo actual.
* **Matching Inteligente:** Notificar a los Investigadores cuyas cualificaciones (**idiomas, área**) coincidan con una nueva Convocatoria.
* **Asignación (Antena):** El DP debe poder seleccionar al candidato óptimo, validando automáticamente la Carga de Trabajo.
* **Control de Entregables:** Módulo de seguimiento con alertas automáticas por *deadlines* y registro de la subida de informes.
* **Gestión Financiera:** Registro de presupuestos, gastos, nóminas y registro de la Compensación.

