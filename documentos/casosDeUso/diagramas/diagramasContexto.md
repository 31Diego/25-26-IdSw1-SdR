# Diagramas de contexto (GIPF – FUNIBER)

Este documento recoge los **diagramas de contexto** del sistema para los dos actores principales: **Coordinador** e **Investigador**.  
Cada diagrama define los **estados de pantalla** y las **transiciones** permitidas mediante acciones (casos de uso) coherentes con el contexto del actor.

---

## Coordinador — Diagrama de contexto

- **Actor**: Coordinador  
- **Objetivo**: Visualizar la navegación completa del coordinador (visión global del sistema) y las acciones disponibles desde cada pantalla.

<div align=center>

|![Diagrama de contexto: Coordinador](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/imagenes/diagramaContextoCoordinador.svg)|
|-|
|Código fuente: [DiagramaContextoCoordinador.puml](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/diagramas/diagramaContextoCoordinador.puml)|

</div>

### Estados principales resumidos
- `SESION_CERRADA` / `PANEL_PRINCIPAL_ABIERTO`
- Accesos desde panel: `OPCIONES_PERFIL_ABIERTO`, `OPCIONES_CARGA_TRABAJO_ABIERTAS`, `PROYECTOS_ABIERTOS`, `INVESTIGADORES_ABIERTOS`, `MIS_PUBLICACIONES_ABIERTAS`, `PUBLICACIONES_ABIERTAS`, `CONVOCATORIAS_ABIERTAS`, `RECOMPENSAS_ABIERTAS`
- Subpantallas de detalle: `PUBLICACION_ABIERTA`, `MI_PUBLICACION_ABIERTA`, `CONVOCATORIA_ABIERTA`, `RECOMPENSA_ABIERTA`, `PROYECTO_ABIERTO`, `ENTREGABLES_ABIERTOS`, `ENTREGABLE_ABIERTO`, `INVESTIGADOR_ABIERTO`, `SOLICITUDES_ELIMINACION_PERFIL_ABIERTAS`, `SOLICITUD_ELIMINACION_PERFIL_ABIERTA`

---

## Investigador — Diagrama de contexto

- **Actor**: Investigador  
- **Objetivo**: Visualizar la navegación del investigador (operación sobre información propia y acceso de consulta) y sus acciones disponibles.

<div align=center>

|![Diagrama de contexto: Investigador](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/imagenes/diagramaContextoInvestigador.svg)|
|-|
|Código fuente: [DiagramaContextoInvestigador.puml](https://github.com/31Diego/25-26-IdSw1-SdR/blob/main/documentos/casosDeUso/diagramas/diagramaContextoInvestigador.puml)|

</div>

### Estados principales resumidos
- `SESION_CERRADA` / `PANEL_PRINCIPAL_ABIERTO`
- Accesos desde panel: `OPCIONES_PERFIL_ABIERTO`, `OPCIONES_CARGA_TRABAJO_ABIERTAS`, `PROYECTOS_ABIERTOS`, `INVESTIGADORES_ABIERTOS`, `MIS_PUBLICACIONES_ABIERTAS`, `PUBLICACIONES_ABIERTAS`, `RECOMPENSAS_ABIERTAS`
- Subpantallas de detalle: `PUBLICACION_ABIERTA`, `MI_PUBLICACION_ABIERTA`, `PROYECTO_ABIERTO`, `ENTREGABLES_ABIERTOS`, `ENTREGABLE_ABIERTO`, `RECOMPENSA_ABIERTA`, `INVESTIGADOR_ABIERTO`

---
