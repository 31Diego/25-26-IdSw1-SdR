# Proyecto FUNIBER – Plataforma interna tipo “LinkedIn”

## 1. Contexto general
El cliente es **FUNIBER (Fundación Universitaria Iberoamericana)**, una institución con varias sedes internacionales que está vinculada a **UNEATLANTICO**.

El área principal involucrada es el **Departamento de Proyectos de Investigación**, que se encarga de gestionar convocatorias, propuestas y proyectos financiados por diferentes entidades (como SODERCAN o la Unión Europea).

La idea general es crear una **plataforma interna estilo LinkedIn**, donde los **investigadores y docentes** puedan tener su perfil, gestionar sus proyectos, controlar convocatorias y hacer seguimiento de todo lo que pasa en el área de investigación.

En resumen: una herramienta que sirva tanto como **sistema de gestión** para el departamento como una **red profesional interna** para los miembros de FUNIBER.

---

## 2. Situación actual y estructura general
Actualmente, los **docentes-investigadores** pueden impartir **hasta 4 asignaturas por cuatrimestre**, lo que equivale a **16 horas semanales**, y **no se puede superar** bajo ningún concepto.

En algunas sedes solo hay investigadores, mientras que en otras los mismos también imparten docencia.

En cuanto a las **compensaciones**, depende del tipo de perfil:

- Si es **solo investigador**: cuando termina un proyecto, recibe **una compensación económica**.
- Si es **investigador y docente**: puede elegir entre  
  1️⃣ una **reducción de horas docentes**, o  
  2️⃣ **una compensación económica**.  

Esta compensación se da **al finalizar el proyecto**, no durante su desarrollo.

---

## 3. Tipología y flujo de los proyectos de investigación
Los proyectos pueden estar financiados por distintas entidades, como:
- **SODERCAN** (proyectos de innovación en Cantabria)
- **La Unión Europea** (proyectos competitivos)

El flujo de trabajo se divide en fases:

1. **Antena**
   - Persona encargada de **detectar convocatorias** interesantes.  
   - También **redacta y presenta** las propuestas.
   - Se encarga de analizar qué convocatorias son relevantes para FUNIBER.

2. **Propuesta**
   - Si se **rechaza**, queda registrada en el sistema como **histórico**, vinculada al investigador responsable.
   - Si se **acepta**, pasa a ser un **proyecto activo**.

3. **Proyecto**
   - Se asignan **dos responsables** para su ejecución.
   - Se gestionan **financiación**, **entregables** y **plazos**.
   - Se definen **roles y responsabilidades**, todo registrado en la plataforma.

---

## 4. Roles dentro de los proyectos
- **Investigador principal**: coordina todo el proyecto y responde ante el Departamento de Proyectos.  
- **Investigadores asociados**: participan directamente en las tareas.  
- **Colaboradores**: no tienen acceso al sistema, pero deben aparecer en el equipo con su sede.  
- **Finanzas**: lleva todo lo económico (nóminas, gastos, presupuestos, compensaciones…).

---

## 5. Requisitos de la herramienta

### 5.1. Gestión de perfiles
Cada investigador/docente tendrá su perfil con:
- Nombre, apellidos, edad, sexo y sede.  
- Código interno de FUNIBER.  
- CV, publicaciones, congresos, proyectos previos.  
- Idiomas y área de investigación.  
- Carga actual (docencia + investigación).  

El sistema debe **controlar automáticamente** que nadie supere las **16 horas semanales**.

---

### 5.2. Gestión de convocatorias
El sistema debe permitir:
- Registrar **todas las convocatorias activas**.  
- Clasificarlas por **tipo de financiación**, fechas, requisitos, etc.  
- **Notificar** a los investigadores cuyo perfil encaje con una convocatoria.  
- Facilitar al Departamento de Proyectos la **asignación de la persona más adecuada**, teniendo en cuenta su carga actual.

---

### 5.3. Gestión de propuestas y proyectos
El flujo básico:
1. La **Antena** presenta la propuesta directamente desde la herramienta.  
2. Si la propuesta se **rechaza**, queda archivada como histórico.  
3. Si se **acepta**, se genera el proyecto activo con toda su información:
   - Datos del proyecto (título, entidad, importe, duración, objetivos…).  
   - Responsables, participantes, colaboradores.  
   - Entregables con fechas límite y seguimiento.  
   - Informes y logros obtenidos.  

El sistema debe:
- Permitir **subir entregables**.  
- Enviar **alertas automáticas** cuando se acerquen los deadlines.  
- Guardar una **memoria histórica** de proyectos anteriores.

---

### 5.4. Gestión financiera y compensaciones
Debe incluir un módulo para:
- Registrar **gastos, presupuestos y nóminas**.  
- Controlar **pagos y compensaciones** por proyectos finalizados.  
- Registrar si el investigador/docente elige **compensación económica** o **reducción de horas docentes**.

---

## 6. Objetivos principales
1. Crear una plataforma completa para el Departamento de Proyectos.  
2. Conectar a investigadores y docentes de todas las sedes.  
3. Identificar rápidamente perfiles adecuados para nuevas convocatorias.  
4. Evitar sobrecargas y duplicidades de tareas.  
5. Centralizar toda la información de proyectos activos e históricos.  
6. Automatizar alertas y seguimientos.  
7. Registrar de forma clara y trazable todas las compensaciones, propuestas y resultados.

---

## 7. Estructura de usuarios del sistema
Los usuarios principales serán:
- Vicerrector/a de Investigación  
- Vicerrectora Académica  
- Rector  
- Personal del Departamento de Proyectos  
- Investigadores / Investigadores-docentes  
- Agentes externos o financiadores (acceso limitado)  
- Colaboradores (registrados, pero sin acceso directo)

El sistema deberá permitir ver **indicadores globales**, como:
- Nº de propuestas presentadas  
- Nº de proyectos financiados  
- Estado actual de cada proyecto (en curso, finalizado, rechazado, etc.)  
- Distribución por sede e investigador  
 