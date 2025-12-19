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

# Actores y Casos de Uso

## Información del artefacto

- **Proyecto**: Plataforma Interna de Investigación de FUNIBER (GIPF)

---

## Introducción

Este documento describe los **actores del sistema** y los **casos de uso asociados** de la Plataforma Interna de Investigación de FUNIBER.  
El objetivo es definir de forma clara las **interacciones fundamentales** entre los actores *Coordinador* e *Investigador* y el sistema, mediante **casos de uso atómicos**, coherentes con los diagramas de contexto y alineados con un enfoque CRUD cuando aplica.

La identificación y estructuración de estos casos de uso sirve como base para la posterior **especificación detallada**, el **prototipado** y la validación funcional del sistema.

---

## Propósito

- Identificar los actores que interactúan con el sistema.
- Definir los casos de uso asociados a cada actor.
- Establecer claramente las responsabilidades de cada rol.
- Proporcionar una base estructurada para la especificación detallada de requisitos.
- Facilitar la trazabilidad entre actores, diagramas de contexto y casos de uso.

---

## Diagramas

- [Diagrama de actores y casos de uso del Coordinador](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/imagenes/cduCoordinador.svg)
- [Diagrama de actores y casos de uso del Investigador](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/imagenes/cduInvestigador.svg)
- [Diagrama de contexto del Coordinador](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/imagenes/diagramaContextoCoordinador.svg)
- [Diagrama de contexto del Investigador](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/imagenes/diagramaContextoInvestigador.svg)

---

## Actores identificados

| Actor | Descripción | Responsabilidades principales |
|--|--|--|
| **Coordinador** | Usuario con funciones de coordinación y supervisión del departamento de proyectos de investigación. | Supervisar proyectos y convocatorias.<br>Gestionar investigadores y su carga de trabajo.<br>Controlar recompensas, entregables y seguimiento global. |
| **Investigador** | Usuario que participa activamente en proyectos de investigación y genera contenidos propios. | Gestionar su perfil y publicaciones.<br>Consultar proyectos propios y entregables.<br>Registrar y actualizar resultados de investigación. |

---

## Casos de uso por actor

### Coordinador

El Coordinador dispone de una visión **global del sistema** y puede actuar sobre todas las entidades relevantes del dominio.

#### Gestión de sesión
- iniciarSesion()
- cerrarSesion()

#### Navegación general
- abrirPanelPrincipal()

#### Perfil
- abrirOpcionesPerfil()
- editarPerfil()
- solicitarEliminacionPerfil()
- abrirSolicitudesEliminacionPerfil()
- abrirSolicitudEliminacionPerfil()

#### Carga de trabajo
- abrirOpcionesCargaTrabajo()
- editarCargaTrabajo()

#### Publicaciones
- abrirPublicaciones()
- abrirPublicacion()
- responderPublicacion()
- editarPublicacion()
- eliminarPublicacion()

#### Mis publicaciones
- abrirMisPublicaciones()
- abrirMiPublicacion()
- crearPublicacion()
- editarPublicacion()
- eliminarPublicacion()

#### Convocatorias
- abrirConvocatorias()
- abrirConvocatoria()
- importarConvocatoria()

#### Recompensas
- abrirRecompensas()
- abrirRecompensa()
- crearRecompensa()
- editarRecompensa()
- eliminarRecompensa()

#### Proyectos
- abrirProyectos()
- abrirProyecto()
- crearProyecto()
- editarProyecto()
- eliminarProyecto()
- agregarInvestigador()
- eliminarInvestigador()
- abrirEntregables()
- abrirEntregable()
- crearEntregable()
- editarEntregable()
- eliminarEntregable()

#### Investigadores
- abrirInvestigadores()
- abrirInvestigador()
- crearInvestigador()

---

### Investigador

El Investigador opera sobre **información propia**, con acceso limitado a consultas globales cuando procede.

#### Gestión de sesión
- iniciarSesion()
- cerrarSesion()

#### Navegación general
- abrirPanelPrincipal()

#### Perfil
- abrirOpcionesPerfil()
- editarPerfil()
- solicitarEliminacionPerfil()

#### Carga de trabajo (individual)
- abrirOpcionesCargaTrabajo()
- editarCargaTrabajo()

#### Publicaciones (común)
- abrirPublicaciones()
- abrirPublicacion()
- responderPublicacion()

#### Mis publicaciones
- abrirMisPublicaciones()
- abrirMiPublicacion()
- crearPublicacion()
- editarPublicacion()
- eliminarPublicacion()

#### Proyectos propios
- abrirProyectos()
- abrirProyecto()
- abrirEntregables()
- abrirEntregable()
- crearEntregable()
- editarEntregable()
- eliminarEntregable()

#### Recompensas
- abrirRecompensas()
- abrirRecompensa()

#### Investigadores (consulta)
- abrirInvestigadores()
- abrirInvestigador()

---

## Características de los casos de uso

### Atomicidad
- Cada caso de uso representa una interacción completa actor–sistema.
- Tiene un inicio y un fin claramente definidos.
- Produce un resultado observable para el actor.
- No se descompone en subcasos de uso.

### Nomenclatura
- Los casos de uso siguen una convención basada en verbos en infinitivo.
- Los nombres reflejan directamente la acción realizada.
- Existe coherencia con el vocabulario del dominio del proyecto.

### Trazabilidad
- Todos los casos de uso están alineados con los diagramas de contexto.
- Cada transición de salida se corresponde con un estado existente.
- Los casos de uso detallados y los prototipos mantienen una correspondencia 1:1.

---

## Consideraciones de diseño

### Separación de responsabilidades
- **Coordinador**: control global, supervisión y toma de decisiones.
- **Investigador**: gestión de información propia y participación en proyectos.

### Cobertura funcional
Los casos de uso cubren el ciclo completo de la actividad investigadora:
1. Identificación de convocatorias.
2. Propuestas y proyectos.
3. Seguimiento de entregables.
4. Publicaciones y resultados.
5. Recompensas y carga de trabajo.

### Extensibilidad
La estructura definida permite:
- Incorporar nuevos roles.
- Añadir nuevos casos de uso.
- Ampliar funcionalidades sin afectar al núcleo del sistema.