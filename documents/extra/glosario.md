# Glosario de la Plataforma Interna de Investigación de FUNIBER

Breve glosario unificado de términos y conceptos utilizados en la Plataforma Interna de Investigación de FUNIBER.  
La tabla recoge la definición y ejemplos o características clave asociadas a cada término, garantizando coherencia con los diagramas de contexto, casos de uso y prototipos del sistema.

| Término | Definición | Ejemplos / Características |
|--|--|--|
| Investigador | Usuario del sistema que desarrolla actividades de investigación y puede publicar contenidos propios. | Accede a proyectos propios, crea y edita publicaciones, consulta recompensas, gestiona sus entregables. |
| Investigador-docente | Investigador que, además de investigación, imparte docencia y tiene límites de carga docente. | Máx. 16 h/semana de docencia; combinación de docencia, investigación y actividades académicas. |
| Coordinador | Usuario responsable de coordinar y supervisar la actividad investigadora. | Define proyectos, asigna investigadores, controla carga de trabajo, gestiona convocatorias y recompensas. |
| Panel principal | Pantalla central de navegación del sistema tras iniciar sesión. | Accesos a proyectos, investigadores, publicaciones, recompensas, perfil y cierre de sesión. |
| Perfil | Conjunto de datos identificativos y académicos de un usuario. | Datos personales, sede, área de investigación, rol, información profesional. |
| Proyecto | Entidad que agrupa actividades de investigación con un objetivo común. | Estado (borrador, en curso, finalizado), fechas, coordinador, equipo investigador. |
| Proyecto abierto | Estado en el que se visualiza el detalle completo de un proyecto. | Datos generales, descripción, equipo, acceso a entregables e investigadores asociados. |
| Entregable | Resultado parcial o final asociado a un proyecto. | Informe, dataset, presentación u otro; tiene fecha límite y estado. |
| Entregables abiertos | Listado de entregables asociados a un proyecto concreto. | Permite filtrar, abrir o crear entregables según permisos. |
| Publicación | Contenido generado por un investigador dentro de la plataforma. | Puede estar en borrador o publicada; tiene visibilidad pública o privada. |
| Mis publicaciones | Listado de publicaciones creadas por un investigador. | Incluye filtros por estado, fecha y título; acceso a creación y edición. |
| Publicaciones | Listado general de publicaciones visibles en la plataforma. | Acceso común para investigadores y coordinadores; permite abrir y responder. |
| Convocatoria | Llamada institucional para la presentación de proyectos de investigación. | Fechas de apertura y cierre, área, entidad financiadora, estado. |
| Recompensa | Reconocimiento económico o académico asociado a la actividad investigadora. | Compensación económica o reducción de carga docente. |
| Carga de trabajo | Distribución semanal de horas de una persona. | Docencia, investigación y actividades académicas; total semanal y márgenes. |
| Opciones de carga de trabajo | Pantalla de consulta y edición de la carga de trabajo. | Vista individual o global según rol; edición controlada por el coordinador. |
| Estado | Situación en la que se encuentra una entidad del sistema. | Proyecto en curso, entregable pendiente, publicación en borrador, etc. |
| Visibilidad | Ámbito de acceso de una publicación. | Pública (comunidad FUNIBER) o privada (autor). |
| Listado | Vista que presenta múltiples entidades de un mismo tipo. | Proyectos, entregables, publicaciones, investigadores. |
| Objeto abierto | Vista detallada de una entidad concreta. | Proyecto abierto, publicación abierta, entregable abierto. |
| Filtro | Criterio aplicado a un listado para acotar resultados. | Por estado, fecha, título, proyecto, investigador. |
| Sesión | Periodo de interacción autenticada de un usuario con el sistema. | Se inicia con iniciarSesion() y finaliza con cerrarSesion(). |
| Transición | Cambio de estado dentro del sistema según el diagrama de contexto. | Ej.: PANEL_PRINCIPAL_ABIERTO → PROYECTOS_ABIERTOS. |
| Caso de uso | Descripción estructurada de una interacción entre actor y sistema. | abrirProyectos(), crearPublicacion(), editarEntregable(). |
| Prototipo | Representación visual de una pantalla del sistema. | Wireframes en notación SALT coherentes con los casos de uso. |
