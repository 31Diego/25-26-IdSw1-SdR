# Detalle y prototipo de casos de uso

#### A continuación se presenta la especificación y los prototipos de cada caso de uso, clasificados por ámbito funcional.

---

## Casos de uso comunes (Coordinador e Investigador)

### Gestión de sesión
- [iniciarSesion](./casos-uso/iniciarSesion.md) – El usuario introduce sus credenciales y accede al panel principal del sistema  
- [cerrarSesion](./casos-uso/cerrarSesion.md) – El usuario cierra la sesión activa y vuelve al estado de sesión cerrada  
- [denegarInicioSesion](./casos-uso/denegarInicioSesion.md) – El sistema bloquea el acceso cuando las credenciales no son válidas  

---

### Perfil
- [abrirOpcionesPerfil](./casos-uso/abrirOpcionesPerfil.md) – El usuario accede al panel de configuración de su perfil  
- [editarPerfil](./casos-uso/editarPerfil.md) – El usuario modifica sus datos personales  
- [solicitarEliminacionPerfil](./casos-uso/solicitarEliminacionPerfil.md) – El usuario solicita la eliminación de su perfil del sistema  
- [abrirOpcionesCargaTrabajo](./casos-uso/abrirOpcionesCargaTrabajo.md) – El usuario accede a la vista de su carga de trabajo  
- [editarCargaTrabajo](./casos-uso/editarCargaTrabajo.md) – El usuario actualiza la información de su carga de trabajo  
- [abrirPanelPrincipal](./casos-uso/abrirPanelPrincipal.md) – El usuario regresa al panel principal desde cualquier vista  

---

### Publicaciones (generales)
- [abrirPublicaciones](./casos-uso/abrirPublicaciones.md) – El usuario accede al listado general de publicaciones  
- [abrirPublicacion](./casos-uso/abrirPublicacion.md) – El usuario abre una publicación concreta  
- [responderPublicacion](./casos-uso/responderPublicacion.md) – El usuario responde o comenta una publicación  

---

### Mis Publicaciones
- [abrirMisPublicaciones](./casos-uso/abrirMisPublicaciones.md) – El usuario accede al listado de sus propias publicaciones  
- [abrirMiPublicacion](./casos-uso/abrirMiPublicacion.md) – El usuario abre una de sus publicaciones  
- [crearPublicacion](./casos-uso/crearPublicacion.md) – El usuario crea una nueva publicación  
- [editarPublicacion](./casos-uso/editarPublicacion.md) – El usuario edita una publicación propia  
- [eliminarPublicacion](./casos-uso/eliminarPublicacion.md) – El usuario elimina una de sus publicaciones  

---

### Proyectos
- [abrirProyectos](./casos-uso/abrirProyectos.md) – El usuario accede al listado de proyectos  
- [abrirProyecto](./casos-uso/abrirProyecto.md) – El usuario accede a un proyecto concreto  

---

### Entregables
- [abrirEntregables](./casos-uso/abrirEntregables.md) – El usuario consulta los entregables de un proyecto  
- [crearEntregable](./casos-uso/crearEntregable.md) – El usuario crea un nuevo entregable  
- [editarEntregable](./casos-uso/editarEntregable.md) – El usuario modifica un entregable existente  
- [eliminarEntregable](./casos-uso/eliminarEntregable.md) – El usuario elimina un entregable  

---

### Investigadores
- [abrirInvestigadores](./casos-uso/abrirInvestigadores.md) – El usuario accede al listado de investigadores  
- [abrirInvestigador](./casos-uso/abrirInvestigador.md) – El usuario consulta el perfil de un investigador  

---

## Casos de uso exclusivos del Coordinador

### Gestión de Proyectos
- [crearProyecto](./casos-uso/crearProyecto.md) – El coordinador registra un nuevo proyecto en el sistema  
- [editarProyecto](./casos-uso/editarProyecto.md) – El coordinador modifica la información de un proyecto  
- [eliminarProyecto](./casos-uso/eliminarProyecto.md) – El coordinador elimina un proyecto existente  
- [agregarInvestigador](./casos-uso/agregarInvestigador.md) – El coordinador asigna un investigador a un proyecto  
- [eliminarInvestigador](./casos-uso/eliminarInvestigador.md) – El coordinador retira un investigador de un proyecto  

---

### Gestión de Investigadores
- [crearInvestigador](./casos-uso/crearInvestigador.md) – El coordinador registra un nuevo investigador en el sistema  
