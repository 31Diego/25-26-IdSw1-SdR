# Proyecto FUNIBER – Avance del Requesitado

## 1. Introducción
El proyecto consiste en el desarrollo de una **plataforma interna para FUNIBER** (Fundación Universitaria Iberoamericana), una institución con varias sedes internacionales vinculada a la **Universidad Europea del Atlántico (UNEATLANTICO)**.

El objetivo es crear una herramienta tipo **“LinkedIn interno”** que permita a los investigadores y docentes de FUNIBER:
- Gestionar sus **perfiles académicos y de investigación**.  
- Controlar **convocatorias y propuestas**.  
- Hacer **seguimiento de proyectos**, entregables y compensaciones.  

En resumen, un sistema que sirva tanto como **gestor de proyectos** para el Departamento de Investigación como **red profesional** para el personal de FUNIBER.

---

## 2. Actores del Sistema

| Actor | Descripción |
|-------|--------------|
| **Investigador** | Participa en proyectos, sube entregables y consulta convocatorias. |
| **Docente-Investigador** | Igual que el investigador, pero con control de carga docente (máximo 16 horas semanales). |
| **Antena** | Persona que detecta convocatorias y presenta propuestas. |
| **Departamento de Proyectos** | Gestiona convocatorias, asigna responsables y da seguimiento a los proyectos. |
| **Vicerrector/a de Investigación** | Supervisa proyectos y aprueba o rechaza propuestas. |
| **Finanzas** | Gestiona los gastos, nóminas y compensaciones. |
| **Colaborador** | Forma parte del equipo del proyecto, pero no tiene acceso directo al sistema. |

---

## 3. Casos de Uso Principales

1. **Gestionar Perfiles**  
   - Los usuarios pueden crear, editar y consultar perfiles con su información académica y profesional.  
   - El sistema controla automáticamente que los docentes no superen 16 h/semana.

2. **Registrar Convocatorias**  
   - El Departamento de Proyectos registra convocatorias activas (tipo, fechas, requisitos, etc.).  
   - El sistema notifica automáticamente a los investigadores cuyos perfiles coincidan.

3. **Presentar Propuestas**  
   - La Antena presenta una propuesta a partir de una convocatoria.  
   - Si se rechaza, se guarda como histórico.

4. **Aprobar o Rechazar Propuestas**  
   - El Vicerrector/a revisa y decide sobre las propuestas.  
   - Las aprobadas pasan a ser proyectos activos.

5. **Crear Proyecto Activo**  
   - El sistema crea un registro con título, responsables, participantes, entregables y plazos.  
   - Se definen roles y responsabilidades.

6. **Subir Entregables y Seguimiento**  
   - Los investigadores suben los entregables del proyecto.  
   - El sistema envía alertas automáticas antes de cada deadline.

7. **Registrar Compensaciones**  
   - Una vez finalizado un proyecto, se registra la compensación:  
     - Reducción de horas docentes, o  
     - Compensación económica.  

---

## 4. Entidades Principales

| Entidad | Descripción | Atributos principales |
|----------|--------------|----------------------|
| **Investigador** | Persona que participa en proyectos. | Nombre, sede, CV, publicaciones, idiomas, carga docente/investigadora. |
| **Proyecto** | Actividad de investigación aprobada. | Título, responsables, duración, objetivos, estado, entregables. |
| **Convocatoria** | Oportunidad de financiación. | Entidad, tipo, requisitos, fechas, presupuesto. |
| **Entregable** | Resultado o documento asociado a un proyecto. | Nombre, fecha límite, estado, responsable. |
| **Compensación** | Beneficio recibido tras completar un proyecto. | Tipo (económica o reducción de horas), monto, fecha. |

---

## 5. Requisitos Funcionales (RF)

1. El sistema debe permitir registrar y actualizar perfiles de usuarios.  
2. El sistema debe controlar automáticamente que ningún docente supere las 16 horas semanales.  
3. El sistema debe permitir registrar y clasificar convocatorias.  
4. El sistema debe notificar automáticamente a los investigadores compatibles con cada convocatoria.  
5. El sistema debe permitir la presentación de propuestas desde la herramienta.  
6. El sistema debe almacenar propuestas rechazadas como histórico.  
7. El sistema debe crear registros de proyectos activos con todos los datos asociados.  
8. El sistema debe permitir subir y consultar entregables con sus fechas límite.  
9. El sistema debe generar alertas automáticas cuando se acerquen los plazos.  
10. El sistema debe registrar compensaciones y permitir elegir entre reducción de horas o compensación económica.

---

## 6. Requisitos No Funcionales (RNF)

1. La interfaz debe ser accesible desde cualquier navegador moderno.  
2. El sistema debe ofrecer acceso multiusuario con roles y permisos diferenciados.  
3. Los datos deben almacenarse de manera segura y trazable.  
4. El sistema debe generar notificaciones automáticas (internas o por correo).  
5. Debe permitir escalar fácilmente para incluir más sedes o usuarios.  
6. Debe mantener disponibilidad mínima del 99 % y tiempos de respuesta razonables.  
7. La interfaz debe ser intuitiva y fácil de usar para personal no técnico.

