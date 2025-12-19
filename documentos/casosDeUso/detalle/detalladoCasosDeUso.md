# Detalle y Prototipo de Casos de Uso (GIPF – FUNIBER)

Esta carpeta contiene la **especificación detallada** y el **prototipado** (PlantUML + SALT) de cada caso de uso identificado en la **Plataforma Interna de Investigación de FUNIBER (GIPF)**.

Los casos de uso están organizados por **actor** y por **módulo funcional**, siguiendo los diagramas de contexto y los diagramas de casos de uso del proyecto.

---

## Casos de uso especificados

> Nota rápida:  
> - El **Investigador** opera sobre información **propia** (proyectos propios, publicaciones propias, entregables de sus proyectos).  
> - El **Coordinador** tiene visibilidad y acciones sobre el conjunto del sistema (incluyendo control centralizado).

---

## Coordinador

### Gestión de sesión
- [iniciarSesion](/documentos/casosDeUso/detalle/coordinador/iniciarSesion/iniciarSesion.md) — Acceso autenticado al sistema
- [cerrarSesion](/documentos/casosDeUso/detalle/coordinador/cerrarSesion/cerrarSesion.md) — Cierre de sesión

### Navegación general
- [abrirPanelPrincipal](/documentos/casosDeUso/detalle/coordinador/abrirPanelPrincipal/abrirPanelPrincipal.md) — Acceso al panel principal

### Perfil
- [abrirOpcionesPerfil](/documentos/casosDeUso/detalle/coordinador/abrirOpcionesPerfil/abrirOpcionesPerfil.md) — Apertura de opciones del perfil
- [editarPerfil](/documentos/casosDeUso/detalle/coordinador/editarPerfil/editarPerfil.md) — Edición de datos de perfil
- [solicitarEliminacionPerfil](/documentos/casosDeUso/detalle/coordinador/solicitarEliminacionPerfil/solicitarEliminacionPerfil.md) — Solicitud de eliminación del perfil
- [abrirSolicitudesEliminacionPerfil](/documentos/casosDeUso/detalle/coordinador/abrirSolicitudesEliminacionPerfil/abrirSolicitudesEliminacionPerfil.md) — Listado de solicitudes de eliminación
- [abrirSolicitudEliminacionPerfil](/documentos/casosDeUso/detalle/coordinador/abrirSolicitudEliminacionPerfil/abrirSolicitudEliminacionPerfil.md) — Consulta de una solicitud concreta

### Carga de trabajo
- [abrirOpcionesCargaTrabajo](/documentos/casosDeUso/detalle/coordinador/abrirOpcionesCargaTrabajo/abrirOpcionesCargaTrabajo.md) — Consulta de carga de trabajo
- [editarCargaTrabajo](/documentos/casosDeUso/detalle/coordinador/editarCargaTrabajo/editarCargaTrabajo.md) — Edición de carga de trabajo

### Publicaciones
- [abrirPublicaciones](/documentos/casosDeUso/detalle/coordinador/abrirPublicaciones/abrirPublicaciones.md) — Listado general de publicaciones
- [abrirPublicacion](/documentos/casosDeUso/detalle/coordinador/abrirPublicacion/abrirPublicacion.md) — Apertura de una publicación
- [responderPublicacion](/documentos/casosDeUso/detalle/coordinador/responderPublicacion/responderPublicacion.md) — Respuesta a una publicación
- [editarPublicacion](/documentos/casosDeUso/detalle/coordinador/editarPublicacion/editarPublicacion.md) — Edición de publicación
- [eliminarPublicacion](/documentos/casosDeUso/detalle/coordinador/eliminarPublicacion/eliminarPublicacion.md) — Eliminación de publicación

### Mis publicaciones
- [abrirMisPublicaciones](/documentos/casosDeUso/detalle/coordinador/abrirMisPublicaciones/abrirMisPublicaciones.md) — Listado de publicaciones propias
- [abrirMiPublicacion](/documentos/casosDeUso/detalle/coordinador/abrirMiPublicacion/abrirMiPublicacion.md) — Apertura de una publicación propia
- [crearPublicacion](/documentos/casosDeUso/detalle/coordinador/crearPublicacion/crearPublicacion.md) — Creación de publicación propia
- [editarPublicacion](/documentos/casosDeUso/detalle/coordinador/editarMiPublicacion/editarPublicacion.md) — Edición de publicación propia
- [eliminarPublicacion](/documentos/casosDeUso/detalle/coordinador/eliminarMiPublicacion/eliminarPublicacion.md) — Eliminación de publicación propia

### Convocatorias
- [abrirConvocatorias](/documentos/casosDeUso/detalle/coordinador/abrirConvocatorias/abrirConvocatorias.md) — Listado de convocatorias
- [abrirConvocatoria](/documentos/casosDeUso/detalle/coordinador/abrirConvocatoria/abrirConvocatoria.md) — Consulta de una convocatoria
- [importarConvocatoria](/documentos/casosDeUso/detalle/coordinador/importarConvocatoria/importarConvocatoria.md) — Importación de convocatoria

### Recompensas
- [abrirRecompensas](/documentos/casosDeUso/detalle/coordinador/abrirRecompensas/abrirRecompensas.md) — Listado de recompensas
- [abrirRecompensa](/documentos/casosDeUso/detalle/coordinador/abrirRecompensa/abrirRecompensa.md) — Consulta de recompensa
- [crearRecompensa](/documentos/casosDeUso/detalle/coordinador/crearRecompensa/crearRecompensa.md) — Creación de recompensa
- [editarRecompensa](/documentos/casosDeUso/detalle/coordinador/editarRecompensa/editarRecompensa.md) — Edición de recompensa
- [eliminarRecompensa](/documentos/casosDeUso/detalle/coordinador/eliminarRecompensa/eliminarRecompensa.md) — Eliminación de recompensa

### Proyectos
- [abrirProyectos](/documentos/casosDeUso/detalle/coordinador/abrirProyectos/abrirProyectos.md) — Listado de proyectos
- [abrirProyecto](/documentos/casosDeUso/detalle/coordinador/abrirProyecto/abrirProyecto.md) — Consulta de un proyecto
- [crearProyecto](/documentos/casosDeUso/detalle/coordinador/crearProyecto/crearProyecto.md) — Creación de proyecto
- [editarProyecto](/documentos/casosDeUso/detalle/coordinador/editarProyecto/editarProyecto.md) — Edición de proyecto
- [eliminarProyecto](/documentos/casosDeUso/detalle/coordinador/eliminarProyecto/eliminarProyecto.md) — Eliminación de proyecto
- [agregarInvestigador](/documentos/casosDeUso/detalle/coordinador/agregarInvestigador/agregarInvestigador.md) — Asignación de investigador a proyecto
- [eliminarInvestigador](/documentos/casosDeUso/detalle/coordinador/eliminarInvestigador/eliminarInvestigador.md) — Retirada de investigador del proyecto
- [abrirEntregables](/documentos/casosDeUso/detalle/coordinador/abrirEntregables/abrirEntregables.md) — Listado de entregables del proyecto
- [abrirEntregable](/documentos/casosDeUso/detalle/coordinador/abrirEntregable/abrirEntregable.md) — Consulta de un entregable
- [crearEntregable](/documentos/casosDeUso/detalle/coordinador/crearEntregable/crearEntregable.md) — Creación de entregable
- [editarEntregable](/documentos/casosDeUso/detalle/coordinador/editarEntregable/editarEntregable.md) — Edición de entregable
- [eliminarEntregable](/documentos/casosDeUso/detalle/coordinador/eliminarEntregable/eliminarEntregable.md) — Eliminación de entregable

### Investigadores
- [abrirInvestigadores](/documentos/casosDeUso/detalle/investigador/abrirInvestigadores/abrirInvestigadores.md) — Listado de investigadores
- [abrirInvestigador](/documentos/casosDeUso/detalle/investigador/abrirInvestigador/abrirInvestigador.md) — Consulta de un investigador
- [crearInvestigador](/documentos/casosDeUso/detalle/investigador/crearInvestigador/crearInvestigador.md) — Registro de investigador

---

## Investigador

### Gestión de sesión
- [iniciarSesion](/documentos/casosDeUso/detalle/investigador/iniciarSesion/iniciarSesion.md) — Acceso autenticado al sistema
- [cerrarSesion](/documentos/casosDeUso/detalle/investigador/cerrarSesion/cerrarSesion.md) — Cierre de sesión

### Navegación general
- [abrirPanelPrincipal](/documentos/casosDeUso/detalle/investigador/abrirPanelPrincipal/abrirPanelPrincipal.md) — Acceso al panel principal

### Perfil
- [abrirOpcionesPerfil](/documentos/casosDeUso/detalle/investigador/abrirOpcionesPerfil/abrirOpcionesPerfil.md) — Apertura de opciones del perfil
- [editarPerfil](/documentos/casosDeUso/detalle/investigador/editarPerfil/editarPerfil.md) — Edición de datos de perfil
- [solicitarEliminacionPerfil](/documentos/casosDeUso/detalle/investigador/solicitarEliminacionPerfil/solicitarEliminacionPerfil.md) — Solicitud de eliminación del perfil

### Carga de trabajo (individual)
- [abrirOpcionesCargaTrabajo](/documentos/casosDeUso/detalle/investigador/abrirOpcionesCargaTrabajo/abrirOpcionesCargaTrabajo.md) — Consulta de carga de trabajo propia
- [editarCargaTrabajo](/documentos/casosDeUso/detalle/investigador/editarCargaTrabajo/editarCargaTrabajo.md) — Edición de carga de trabajo propia (según contexto del actor)

### Publicaciones (común)
- [abrirPublicaciones](/documentos/casosDeUso/detalle/investigador/abrirPublicaciones/abrirPublicaciones.md) — Listado general de publicaciones
- [abrirPublicacion](/documentos/casosDeUso/detalle/investigador/abrirPublicacion/abrirPublicacion.md) — Apertura de una publicación
- [responderPublicacion](/documentos/casosDeUso/detalle/investigador/responderPublicacion/responderPublicacion.md) — Respuesta a una publicación

### Mis publicaciones (propias)
- [abrirMisPublicaciones](/documentos/casosDeUso/detalle/investigador/abrirMisPublicaciones/abrirMisPublicaciones.md) — Listado de publicaciones propias
- [abrirMiPublicacion](/documentos/casosDeUso/detalle/investigador/abrirMiPublicacion/abrirMiPublicacion.md) — Apertura de una publicación propia
- [crearPublicacion](/documentos/casosDeUso/detalle/investigador/crearPublicacion/crearPublicacion.md) — Creación de publicación
- [editarPublicacion](/documentos/casosDeUso/detalle/investigador/editarPublicacion/editarPublicacion.md) — Edición de publicación propia
- [eliminarPublicacion](/documentos/casosDeUso/detalle/investigador/eliminarPublicacion/eliminarPublicacion.md) — Eliminación de publicación propia

### Proyectos (propios)
- [abrirProyectos](/documentos/casosDeUso/detalle/investigador/abrirProyectos/abrirProyectos.md) — Listado de proyectos propios
- [abrirProyecto](/documentos/casosDeUso/detalle/investigador/abrirProyecto/abrirProyecto.md) — Consulta de proyecto propio
- [abrirEntregables](/documentos/casosDeUso/detalle/investigador/abrirEntregables/abrirEntregables.md) — Listado de entregables del proyecto
- [abrirEntregable](/documentos/casosDeUso/detalle/investigador/abrirEntregable/abrirEntregable.md) — Consulta de entregable
- [crearEntregable](/documentos/casosDeUso/detalle/investigador/crearEntregable/crearEntregable.md) — Creación de entregable
- [editarEntregable](/documentos/casosDeUso/detalle/investigador/editarEntregable/editarEntregable.md) — Edición de entregable
- [eliminarEntregable](/documentos/casosDeUso/detalle/investigador/eliminarEntregable/eliminarEntregable.md) — Eliminación de entregable
- [abrirProyecto](/documentos/casosDeUso/detalle/investigador/abrirProyecto/abrirProyecto.md) — Volver al proyecto desde entregables

### Recompensas
- [abrirRecompensas](/documentos/casosDeUso/detalle/investigador/abrirRecompensas/abrirRecompensas.md) — Listado de recompensas propias
- [abrirRecompensa](/documentos/casosDeUso/detalle/investigador/abrirRecompensa/abrirRecompensa.md) — Consulta de una recompensa

### Investigadores (consulta)
- [abrirInvestigadores](/documentos/casosDeUso/detalle/investigador/abrirInvestigadores/abrirInvestigadores.md) — Listado de investigadores
- [abrirInvestigador](/documentos/casosDeUso/detalle/investigador/abrirInvestigador/abrirInvestigador.md) — Consulta de un investigador

---

## Estructura de cada caso de uso

Cada carpeta de caso de uso contiene:

- **README.md** — Especificación completa del caso de uso
- **especificacion.puml** — Diagrama de especificación (detallado) en PlantUML
- **prototipo.puml** — Wireframes de prototipado en SALT

---

## Metodología aplicada

- **Coherencia con diagramas de contexto:** no se definen transiciones fuera del contexto.
- **Vocabulario controlado:** acciones del actor y del sistema según el estándar del proyecto.
- **Confirmar vs cancelar:**  
  - Confirmar/Guardar → vuelve al objeto abierto  
  - Cancelar → vuelve al listado
- **Trazabilidad:** las salidas indican la transición.
- **Consistencia 1:1:** campos y botones del prototipo coinciden con el detallado.
