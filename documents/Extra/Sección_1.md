# 📋 Documento de Requisitos – Plataforma Interna FUNIBER

## 1. Contexto general

El cliente es **FUNIBER** (*Fundación Universitaria Iberoamericana*), una institución académica con presencia en múltiples sedes internacionales y vinculación formal con la **Universidad Europea del Atlántico (UNEATLANTICO)**.

El área principal involucrada en este proyecto es el **Departamento de Proyectos de Investigación**, responsable de gestionar todo el ciclo de vida de las iniciativas de investigación: desde la identificación de convocatorias externas hasta la ejecución, seguimiento y cierre de proyectos financiados por entidades como **SODERCAN** (proyectos de innovación en Cantabria) o programas competitivos de la **Unión Europea**.

La visión del cliente es desarrollar una **plataforma interna tipo “LinkedIn”**, pensada exclusivamente para la comunidad de investigadores y docentes de FUNIBER. Esta herramienta debe permitir:

- Crear y mantener **perfiles profesionales** actualizados.
- Gestionar de forma centralizada **convocatorias, propuestas y proyectos activos**.
- Realizar un **seguimiento continuo** de entregables, plazos y compensaciones.
- Facilitar la **colaboración entre sedes** y la visibilidad de perfiles relevantes.
- Evitar sobrecargas de trabajo mediante un control automático de la carga docente e investigadora.

En resumen, se busca una solución dual:  
🔹 Por un lado, un **sistema de gestión robusto** para el Departamento de Proyectos.  
🔹 Por otro, una **red profesional interna** que conecte a investigadores, docentes y equipos de trabajo en todo el ecosistema FUNIBER.

---

## 2. Estructura organizativa y reglas de negocio

### 2.1. Tipos de perfiles

- **Investigador exclusivo**:  
  - No imparte docencia.  
  - Al finalizar un proyecto, recibe **compensación económica**.

- **Docente-investigador**:  
  - Imparte docencia (máximo **4 asignaturas por cuatrimestre**, equivalentes a **16 horas semanales**).  
  - Al finalizar un proyecto, puede elegir entre:  
    1. **Compensación económica**, o  
    2. **Reducción de carga docente** en el siguiente cuatrimestre.  

> **Regla crítica**: Nadie puede superar las 16 horas semanales de docencia. El sistema debe validar esta restricción antes de asignar nuevas responsabilidades.

### 2.2. Sedes

- Algunas sedes tienen **solo investigadores**.  
- Otras tienen **docentes que también investigan**.  
- La plataforma debe funcionar de forma unificada en **todas las sedes**.

---

## 3. Flujo de trabajo de los proyectos

El ciclo de vida de un proyecto se divide en tres fases:

### 3.1. Antena
- El **Departamento de Proyectos** o un investigador identifica una **convocatoria** relevante.
- Se analiza su alineación con las líneas de investigación de FUNIBER.
- Se notifica a los perfiles adecuados según especialidad, sede y disponibilidad.

### 3.2. Propuesta
- Un investigador (o equipo) redacta y envía una **propuesta** a la entidad financiadora.
- Estados posibles:  
  - **Pendiente**  
  - **Aceptada** → pasa a ser un proyecto activo  
  - **Rechazada** → queda archivada como histórico, vinculada al autor

### 3.3. Proyecto
- Una vez aceptada, la propuesta se convierte en un **proyecto activo**.
- Se asignan:
  - **1 Investigador principal** (responsable ante el Departamento de Proyectos)
  - **Investigadores asociados**
  - **Colaboradores externos** (registrados, pero sin acceso al sistema)
- Se gestionan:
  - Entregables con fechas límite
  - Informes periódicos
  - Presupuesto y compensaciones
- Al finalizar, se registra la **compensación elegida** y se archiva el proyecto.

---

## 4. Roles de usuario

| Rol | Acceso |
|-----|--------|
| **Vicerrector/a de Investigación** | Vista global: estadísticas, todos los proyectos, compensaciones |
| **Vicerrectora Académica** | Acceso a carga docente, compensaciones por reducción de horas |
| **Rector** | Visión estratégica: indicadores clave |
| **Departamento de Proyectos** | Gestión completa: convocatorias, propuestas, proyectos, notificaciones |
| **Investigador / Docente-investigador** | Solo sus propios proyectos, propuestas y perfil |
| **Colaboradores externos** | **No tienen acceso al sistema**, pero aparecen en la ficha del proyecto |
| **Entidades financiadoras** | Solo visibles como metadato (nombre, tipo), sin acceso |

---

## 5. Requisitos funcionales

### 5.1. Gestión de perfiles
- Cada usuario tiene un perfil con:
  - Nombre, apellidos, edad, sexo, sede
  - Código interno FUNIBER
  - CV, publicaciones, congresos, proyectos anteriores
  - Idiomas y área de investigación
  - Carga actual (docencia + investigación)
- El sistema **bloquea automáticamente** la asignación de nuevas tareas si se superan las 16 horas semanales de docencia.

### 5.2. Gestión de convocatorias
- Registrar convocatorias con:
  - Título, entidad financiadora, tipo, fechas, requisitos
- Clasificar por categoría, sede, área temática
- Notificar a investigadores cuyo perfil coincida
- Permitir al Departamento de Proyectos asignar responsables según disponibilidad

### 5.3. Gestión de propuestas y proyectos
- Crear propuestas directamente en la plataforma
- Registrar estado: *Pendiente / Aceptada / Rechazada*
- Al aceptarse, generar un proyecto con:
  - Título, duración, importe, objetivos
  - Investigador principal y equipo
  - Entregables con fechas límite
- Subir entregables y marcar como completados
- Alertas automáticas antes de fechas límite
- Historial completo de proyectos finalizados o rechazados

### 5.4. Gestión financiera y compensaciones
- Registrar tipo de compensación al finalizar un proyecto:
  - Económica (monto)
  - Reducción docente (número de horas)
- Vincular compensación al investigador y al proyecto
- Generar reportes para el área de Finanzas

### 5.5. Indicadores y estadísticas
La plataforma debe mostrar, al menos:
- Número de propuestas presentadas
- % de propuestas aceptadas
- Proyectos activos por sede
- Estado de cada proyecto (activo, finalizado, fallido)
- Carga de trabajo por investigador

---

## 6. Objetivos principales

- ✅ Centralizar toda la información de investigación en una única plataforma.
- ✅ Evitar sobrecargas y duplicidades mediante control automático de carga.
- ✅ Agilizar la identificación de perfiles adecuados para nuevas convocatorias.
- ✅ Garantizar trazabilidad total: desde la convocatoria hasta la compensación.
- ✅ Fomentar la colaboración entre sedes mediante una red profesional interna.
- ✅ Automatizar recordatorios, alertas y reportes clave.

---

