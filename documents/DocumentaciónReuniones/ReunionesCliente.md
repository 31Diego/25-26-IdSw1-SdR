# Documentación de las reuniones con el cliente del proyecto de Gestión de Investigación FUNIBER

## 1. Contexto General
* **Cliente:** Fundación Universitaria Iberoamericana (FUNIBER).
* **Unidad Responsable:** Departamento de Proyectos de Investigación.
* **Objetivo:** Desarrollar una plataforma interna tipo "LinkedIn" para investigadores y docentes que centralice la gestión de perfiles, proyectos, convocatorias y entregables.
* **Alcance:** Conectar investigadores y docentes de todas las sedes internacionales.

## 2. Reglas de Negocio

### Carga Laboral
* **Límite Docente:** Los docentes tienen un límite estricto de **16 horas semanales** (equivalente a 4 asignaturas).
* **Validación:** El sistema debe controlar que no se supere este límite al asignar proyectos.

### Sistema de Compensaciones
La compensación se otorga únicamente al **finalizar** el proyecto.
* **Investigador (sin docencia):** Recibe compensación económica.
* **Investigador-Docente:** Puede elegir entre:
    * Reducción de horas docentes.
    * Compensación económica.

## 3. Roles y Actores (Nota de reuniones iniciales)

* **Departamento de Proyectos:** Coordina la gestión, busca convocatorias y revisa propuestas.
* **Investigador Principal:** Coordina el proyecto y responde ante el departamento.
* **Investigadores Asociados:** Ejecutan tareas dentro del proyecto.
* **Asociado:** Nuevo rol definido como un docente que no es investigador *(Nota reunión 21/11)*.
* **Colaboradores:** Personal externo que figura en el equipo pero **no tiene acceso** a la herramienta.
* **Finanzas:** Gestiona nóminas y gastos.

## 4. Flujo de Trabajo (Workflow)

### Fase 1: Antena (Proceso)
* **Definición:** Proceso de búsqueda de convocatorias y detección de oportunidades de financiación (ej. SODERCAN, UE).
* **Responsable:** Es una tarea del Departamento de Proyectos (cualquier persona del dpto.), no un cargo único *(Nota reunión 21/11)*.

### Fase 2: Propuesta
1. Se elabora y presenta la propuesta.
2. Si es **rechazada**, se guarda en el histórico.
3. Si es **aceptada**, se convierte en Proyecto Activo.

### Fase 3: Proyecto Activo
* **Priorización:** Se enfoca según las fechas límite (*deadlines*) de los entregables *(Nota reunión 21/11)*.
* **Seguimiento:** Control de entregables y alertas de plazos.
* **Estados del Proyecto** *(Actualizado reunión 21/11)*:
    * *Planificado* → Cambia a **Aprobado**.
    * *Cancelado* → Cambia a **Denegado**.

## 5. Requisitos Funcionales

### Gestión de Perfiles
El sistema debe registrar y permitir filtrar por:
* Datos personales, sede y código interno.
* Currículum integrado (publicaciones, congresos últimos 2 años).
* Carga actual de docencia e investigación.

### Gestión de Convocatorias
* Registro de convocatorias activas.
* Selección de candidatos basada en perfil y carga de trabajo actual.

### Histórico y Trazabilidad
* Registro de propuestas ganadas y perdidas.
* Memoria histórica de proyectos para consultas futuras.

## 6. Notas Adicionales

* **Herramientas actuales:** Gestión mediante Google Drive y comunicación por correo electrónico *(Confirmado reunión 21/11)*.
* **Comunicación:** Las llamadas son un recurso de último uso *(Nota reunión 21/11)*.
* **Validación:** Existe una revisión manual por parte del Departamento de Proyectos antes de la validación en plataforma *(Nota reunión 21/11)*.