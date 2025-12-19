<h1 align="center">FUNIBER — Plataforma Interna de Investigación</h1>

<p align="center">
  <img src="./documentos/imagenes/LogoGIPF.png" alt="Logo GIPF - FUNIBER Platform" width="200">
</p>

<div align="center">

[![](https://img.shields.io/badge/-Inicio-0A3B64?style=for-the-badge&logo=github&logoColor=white)](/README.md)
[![](https://img.shields.io/badge/-Modelo_del_Dominio-0A3B64?style=for-the-badge&logo=drawio&logoColor=white)](/documentos/modeloDelDominio/modeloDominio.md)
[![](https://img.shields.io/badge/-Actores_y_casos_de_uso-0A3B64?style=for-the-badge&logo=group&logoColor=white)](/documentos/casosDeUso/casosDeUso.ms)

[![](https://img.shields.io/badge/-Detallado_Casos_de_Uso-0A3B64?style=for-the-badge&logo=notepad&logoColor=white)](/documents/CasosDeUso/DetalladoCasosDeUso/)
[![](https://img.shields.io/badge/-Diagrama_de_Contexto-0A3B64?style=for-the-badge&logo=flowchart&logoColor=white)](/documents/CasosDeUso/DiagramaDeContexto/)
[![](https://img.shields.io/badge/-Prototipos-0A3B64?style=for-the-badge&logo=figma&logoColor=white)](/documents/CasosDeUso/Prototipos/)
[![](https://img.shields.io/badge/-Reuniones-0A3B64?style=for-the-badge&logo=google-meet&logoColor=white)](/documents/Reuniones/)
[![](https://img.shields.io/badge/-Priorización-0A3B64?style=for-the-badge&logo=priority&logoColor=white)](/documents/CasosDeUso/PriorizaciónCasosDeUso.md)
[![](https://img.shields.io/badge/-Rúbrica-0A3B64?style=for-the-badge&logo=checklist&logoColor=white)](https://github.com/mmasias/25-26-IdSw1-SdR/blob/main/documents/Rubrica.md)

</div>


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
- [iniciarSesion](iniciarSesion/) — Acceso autenticado al sistema
- [cerrarSesion](cerrarSesion/) — Cierre de sesión

### Navegación general
- [abrirPanelPrincipal](abrirPanelPrincipal/) — Acceso al panel principal

### Perfil
- [abrirOpcionesPerfil](abrirOpcionesPerfil/) — Apertura de opciones del perfil
- [editarPerfil](editarPerfil/) — Edición de datos de perfil
- [solicitarEliminacionPerfil](solicitarEliminacionPerfil/) — Solicitud de eliminación del perfil
- [abrirSolicitudesEliminacionPerfil](abrirSolicitudesEliminacionPerfil/) — Listado de solicitudes de eliminación
- [abrirSolicitudEliminacionPerfil](abrirSolicitudEliminacionPerfil/) — Consulta de una solicitud concreta

### Carga de trabajo
- [abrirOpcionesCargaTrabajo](abrirOpcionesCargaTrabajo/) — Consulta de carga de trabajo
- [editarCargaTrabajo](editarCargaTrabajo/) — Edición de carga de trabajo

### Publicaciones
- [abrirPublicaciones](abrirPublicaciones/) — Listado general de publicaciones
- [abrirPublicacion](abrirPublicacion/) — Apertura de una publicación
- [responderPublicacion](responderPublicacion/) — Respuesta a una publicación
- [editarPublicacion](editarPublicacion/) — Edición de publicación
- [eliminarPublicacion](eliminarPublicacion/) — Eliminación de publicación

### Mis publicaciones
- [abrirMisPublicaciones](abrirMisPublicaciones/) — Listado de publicaciones propias
- [abrirMiPublicacion](abrirMiPublicacion/) — Apertura de una publicación propia
- [crearPublicacion](crearPublicacion/) — Creación de publicación propia
- [editarPublicacion](editarPublicacion/) — Edición de publicación propia
- [eliminarPublicacion](eliminarPublicacion/) — Eliminación de publicación propia

### Convocatorias
- [abrirConvocatorias](abrirConvocatorias/) — Listado de convocatorias
- [abrirConvocatoria](abrirConvocatoria/) — Consulta de una convocatoria
- [importarConvocatoria](importarConvocatoria/) — Importación de convocatoria

### Recompensas
- [abrirRecompensas](abrirRecompensas/) — Listado de recompensas
- [abrirRecompensa](abrirRecompensa/) — Consulta de recompensa
- [crearRecompensa](crearRecompensa/) — Creación de recompensa
- [editarRecompensa](editarRecompensa/) — Edición de recompensa
- [eliminarRecompensa](eliminarRecompensa/) — Eliminación de recompensa

### Proyectos
- [abrirProyectos](abrirProyectos/) — Listado de proyectos
- [abrirProyecto](abrirProyecto/) — Consulta de un proyecto
- [crearProyecto](crearProyecto/) — Creación de proyecto
- [editarProyecto](editarProyecto/) — Edición de proyecto
- [eliminarProyecto](eliminarProyecto/) — Eliminación de proyecto
- [agregarInvestigador](agregarInvestigador/) — Asignación de investigador a proyecto
- [eliminarInvestigador](eliminarInvestigador/) — Retirada de investigador del proyecto
- [abrirEntregables](abrirEntregables/) — Listado de entregables del proyecto
- [abrirEntregable](abrirEntregable/) — Consulta de un entregable
- [crearEntregable](crearEntregable/) — Creación de entregable
- [editarEntregable](editarEntregable/) — Edición de entregable
- [eliminarEntregable](eliminarEntregable/) — Eliminación de entregable

### Investigadores
- [abrirInvestigadores](abrirInvestigadores/) — Listado de investigadores
- [abrirInvestigador](abrirInvestigador/) — Consulta de un investigador
- [crearInvestigador](crearInvestigador/) — Registro de investigador

---

## Investigador

### Gestión de sesión
- [iniciarSesion](iniciarSesion/) — Acceso autenticado al sistema
- [cerrarSesion](cerrarSesion/) — Cierre de sesión

### Navegación general
- [abrirPanelPrincipal](abrirPanelPrincipal/) — Acceso al panel principal

### Perfil
- [abrirOpcionesPerfil](abrirOpcionesPerfil/) — Apertura de opciones del perfil
- [editarPerfil](editarPerfil/) — Edición de datos de perfil
- [solicitarEliminacionPerfil](solicitarEliminacionPerfil/) — Solicitud de eliminación del perfil

### Carga de trabajo (individual)
- [abrirOpcionesCargaTrabajo](abrirOpcionesCargaTrabajo/) — Consulta de carga de trabajo propia
- [editarCargaTrabajo](editarCargaTrabajo/) — Edición de carga de trabajo propia (según contexto del actor)

### Publicaciones (común)
- [abrirPublicaciones](abrirPublicaciones/) — Listado general de publicaciones
- [abrirPublicacion](abrirPublicacion/) — Apertura de una publicación
- [responderPublicacion](responderPublicacion/) — Respuesta a una publicación

### Mis publicaciones (propias)
- [abrirMisPublicaciones](abrirMisPublicaciones/) — Listado de publicaciones propias
- [abrirMiPublicacion](abrirMiPublicacion/) — Apertura de una publicación propia
- [crearPublicacion](crearPublicacion/) — Creación de publicación
- [editarPublicacion](editarPublicacion/) — Edición de publicación propia
- [eliminarPublicacion](eliminarPublicacion/) — Eliminación de publicación propia

### Proyectos (propios)
- [abrirProyectos](abrirProyectos/) — Listado de proyectos propios
- [abrirProyecto](abrirProyecto/) — Consulta de proyecto propio
- [abrirEntregables](abrirEntregables/) — Listado de entregables del proyecto
- [abrirEntregable](abrirEntregable/) — Consulta de entregable
- [crearEntregable](crearEntregable/) — Creación de entregable
- [editarEntregable](editarEntregable/) — Edición de entregable
- [eliminarEntregable](eliminarEntregable/) — Eliminación de entregable
- [abrirProyecto](abrirProyecto/) — Volver al proyecto desde entregables

### Recompensas
- [abrirRecompensas](abrirRecompensas/) — Listado de recompensas propias
- [abrirRecompensa](abrirRecompensa/) — Consulta de una recompensa

### Investigadores (consulta)
- [abrirInvestigadores](abrirInvestigadores/) — Listado de investigadores
- [abrirInvestigador](abrirInvestigador/) — Consulta de un investigador

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