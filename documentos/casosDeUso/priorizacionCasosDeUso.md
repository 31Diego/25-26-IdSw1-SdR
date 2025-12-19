<h1 align="center">FUNIBER — Plataforma Interna de Investigación</h1>

<div align="center">

[![](https://img.shields.io/badge/-Inicio-0A3B64?style=for-the-badge&logo=github&logoColor=white)](/README.md)
[![](https://img.shields.io/badge/-Modelo_del_Dominio-0A3B64?style=for-the-badge&logo=drawio&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/modeloDelDominio/modeloDominio.md)
[![](https://img.shields.io/badge/-Actores_y_casos_de_uso-0A3B64?style=for-the-badge&logo=group&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/casosDeUso.md)
[![](https://img.shields.io/badge/-Glosario-0A3B64?style=for-the-badge&logo=notepad&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/modeloDelDominio/documentos/vocabulario.md)

[![](https://img.shields.io/badge/-Detallado_y_Prototipos-0A3B64?style=for-the-badge&logo=notepad&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/detalle/detalladoYPrototipos.md)
[![](https://img.shields.io/badge/-Diagrama_de_Contexto-0A3B64?style=for-the-badge&logo=flowchart&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/diagramas/diagramasContexto.md)
[![](https://img.shields.io/badge/-Reuniones-0A3B64?style=for-the-badge&logo=google-meet&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/reuniones/reuniones.md)
[![](https://img.shields.io/badge/-Priorización-0A3B64?style=for-the-badge&logo=priority&logoColor=white)](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/priorizacionCasosDeUso.md)
[![](https://img.shields.io/badge/-Rúbrica-0A3B64?style=for-the-badge&logo=checklist&logoColor=white)](https://github.com/mmasias/25-26-IdSw1-SdR/blob/main/documents/l'Rubrica.md)

</div>

# Priorización de Casos de Uso  

Este documento establece una **priorización** de los casos de uso identificados en el sistema, con el objetivo de definir un **orden de implementación recomendado**.

La priorización se ha realizado atendiendo a:
- Dependencias funcionales.
- Valor aportado al negocio.
- Necesidad para la navegación y uso básico del sistema.

Se distinguen tres niveles:
- **P0 — Imprescindible**: sin estos casos de uso el sistema no es utilizable.
- **P1 — Núcleo funcional**: funcionalidades principales del dominio.
- **P2 — Complementario / administrativo**: casos de uso de soporte o menor frecuencia.

---

## Coordinador

El **Coordinador** dispone de una visión global del sistema y puede actuar sobre todas las entidades relevantes del dominio.

### P0 — Base del sistema
- iniciarSesion()
- cerrarSesion()
- abrirPanelPrincipal()
- abrirOpcionesPerfil()
- editarPerfil()
- abrirOpcionesCargaTrabajo()

---

### P1 — Núcleo funcional

#### Proyectos y entregables
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

---

### P2 — Gestión y administración

#### Recompensas
- abrirRecompensas()
- abrirRecompensa()
- crearRecompensa()
- editarRecompensa()
- eliminarRecompensa()

#### Investigadores
- abrirInvestigadores()
- abrirInvestigador()
- crearInvestigador()

#### Gestión de perfil (casos poco frecuentes)
- solicitarEliminacionPerfil()
- abrirSolicitudesEliminacionPerfil()
- abrirSolicitudEliminacionPerfil()

---

## Investigador

El **Investigador** opera sobre información propia, con acceso limitado a consultas globales cuando procede.

### P0 — Base del sistema
- iniciarSesion()
- cerrarSesion()
- abrirPanelPrincipal()
- abrirOpcionesPerfil()
- editarPerfil()
- abrirOpcionesCargaTrabajo()

---

### P1 — Núcleo funcional

#### Proyectos propios y entregables
- abrirProyectos()
- abrirProyecto()
- abrirEntregables()
- abrirEntregable()
- crearEntregable()
- editarEntregable()
- eliminarEntregable()

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

---

### P2 — Funcionalidades complementarias

#### Recompensas
- abrirRecompensas()
- abrirRecompensa()

#### Investigadores (consulta)
- abrirInvestigadores()
- abrirInvestigador()

#### Gestión de perfil
- solicitarEliminacionPerfil()

---
