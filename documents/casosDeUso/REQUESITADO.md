# Proyecto FUNIBER – Requesitado

## Introducción
El proyecto consiste en el desarrollo de una **plataforma interna para FUNIBER** (Fundación Universitaria Iberoamericana), vinculada a la **Universidad Europea del Atlántico (UNEATLANTICO)**.

El objetivo es crear una herramienta tipo **“LinkedIn interno”** que centralice la información de los investigadores y docentes, sus proyectos, convocatorias, propuestas y entregables.  
De esta forma, la plataforma permitirá mejorar la **organización, trazabilidad y comunicación** dentro del Departamento de Proyectos de Investigación.

---

## Actores del sistema

| Actor | Descripción |
|-------|--------------|
| **Investigador** | Participa en proyectos, sube entregables y puede ser propuesto para nuevas convocatorias. |
| **Docente-Investigador** | Además de investigar, imparte docencia. El sistema controla que no supere las 16 horas semanales. |
| **Antena** | Detecta convocatorias de interés y presenta propuestas. |
| **Departamento de Proyectos** | Supervisa convocatorias, asigna responsables y da seguimiento a los proyectos. |
| **Vicerrector/a de Investigación** | Revisa las propuestas y aprueba o rechaza proyectos. |
| **Finanzas** | Controla gastos, nóminas y compensaciones. |
| **Colaborador** | Forma parte del equipo de un proyecto, pero sin acceso directo al sistema. |

---

## Descripción de los casos de uso principales

### Registrar perfil de usuario
La plataforma permite registrar un nuevo perfil de investigador o docente con su información básica (nombre, sede, área de investigación, currículum, publicaciones, idiomas, proyectos previos, etc.).  
El perfil queda disponible en el sistema y puede ser actualizado o consultado más adelante.

### Actualizar información de perfil
Cada usuario puede modificar sus datos cuando sea necesario, por ejemplo al añadir nuevas publicaciones o proyectos.  
El sistema controla de forma automática que los docentes no superen las **16 horas semanales** de carga docente.

### Registrar convocatorias
El Departamento de Proyectos puede añadir al sistema todas las convocatorias activas, indicando la entidad que financia, las fechas, los requisitos y el tipo de financiación.  
El sistema identifica los perfiles que encajan con cada convocatoria y envía notificaciones a los investigadores o docentes correspondientes.

### Presentar propuestas
La persona que actúa como Antena puede elaborar y enviar propuestas directamente desde la plataforma.  
Si una propuesta es rechazada, el sistema la guarda como histórico.  
Si es aceptada, se convierte en un proyecto activo y se le asignan responsables.

### Crear y administrar proyectos activos
Cuando una propuesta es aprobada, se genera un registro de proyecto que incluye:
- Información básica (título, objetivos, duración, entidad financiadora).  
- Investigador principal y equipo asociado.  
- Entregables con sus fechas límite.  
- Seguimiento del progreso.  

El sistema envía **alertas automáticas** cuando se acercan los plazos o existen retrasos, y guarda los proyectos finalizados en una memoria histórica accesible.

### Subir entregables y realizar seguimiento
Los investigadores pueden subir los entregables correspondientes a su proyecto (informes, documentos, resultados, etc.).  
El sistema marca automáticamente su estado (pendiente, entregado o retrasado) y notifica tanto al investigador como al departamento responsable.

### Registrar compensaciones
Cuando un proyecto se finaliza, se registra la compensación correspondiente para los participantes:  
- En el caso de los investigadores, se aplica una **compensación económica**.  
- En el caso de los investigadores-docentes, pueden elegir entre **compensación económica** o **reducción de horas docentes**.

### Consultar proyectos y convocatorias
Todos los usuarios con permisos pueden consultar proyectos activos o pasados, así como convocatorias abiertas o finalizadas.  
El sistema ofrece filtros por sede, investigador, estado del proyecto o tipo de financiación.

---

## Entidades principales del sistema

| Entidad | Descripción | Atributos principales |
|----------|--------------|----------------------|
| **Usuario** | Representa a investigadores y docentes. | Nombre, sede, CV, publicaciones, idiomas, carga docente/investigadora. |
| **Proyecto** | Contiene la información de los proyectos aprobados. | Título, responsables, fechas, estado, entregables, resultados. |
| **Convocatoria** | Oportunidad de financiación o investigación. | Entidad, tipo, requisitos, fechas, presupuesto. |
| **Entregable** | Documento o resultado de un proyecto. | Título, fecha límite, estado, responsable. |
| **Compensación** | Registro del beneficio tras completar un proyecto. | Tipo (económica o reducción de horas), monto, fecha. |


