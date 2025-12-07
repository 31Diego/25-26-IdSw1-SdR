# Detalle y prototipo de casos de uso

#### A continuación la especificación y los prototipos de cada caso de uso, clasificados por ámbito

## Casos de uso comunes (Coordinador e Investigador)

### Gestión de sesión 
- [iniciarSesion](link) - El usuario introduce credenciales correctas y accede a su perfil  
- [cerrarSesion](link) - El usuario finaliza su sesión y vuelve al estado de sesión cerrada  
- [denegarInicioSesion](link) - El sistema rechaza un intento de inicio de sesión cuando las credenciales no son válidas  

---

### Perfil 
- [abrirOpcionesPerfil](link) - El usuario accede a su menú de configuración personal  
- [abrirOpcionesCargaTrabajo](link) - El usuario abre el panel para gestionar o visualizar su carga de trabajo  
- [abrirProyectos](link) - El usuario accede al listado de proyectos  
- [abrirInvestigadores](link) - El usuario accede al listado de investigadores  
- [abrirMisPublicaciones](link) - El usuario accede a sus propias publicaciones  
- [abrirPublicaciones](link) - El usuario accede al listado general de publicaciones  
- [editarPerfil](link) - El usuario modifica sus datos personales  
- [eliminarPerfil](link) - El usuario elimina su perfil del sistema  
- [abrirPerfil](link) - El usuario regresa a la vista principal de su perfil  

---

### Publicaciones (generales) 
- [abrirPublicacion](link) - El usuario abre una publicación específica  
- [responderPublicacion](link) - El usuario añade una respuesta o comentario  
- [abrirPublicaciones](link) - El usuario vuelve al listado general de publicaciones  

---

### Mis Publicaciones 
- [abrirMiPublicacion](link) - El usuario abre una de sus propias publicaciones  
- [crearPublicacion](link) - El usuario crea una nueva publicación  
- [editarPublicacion](link) - El usuario edita una de sus publicaciones  
- [eliminarPublicacion](link) - El usuario elimina una de sus publicaciones  
- [abrirMisPublicaciones](link) - El usuario vuelve al listado de sus publicaciones  

---

### Proyectos (comunes) 
- [abrirProyecto](link) - El usuario abre un proyecto concreto  
- [abrirEntregables](link) - El usuario consulta los entregables del proyecto  
- [abrirProyectos](link) - El usuario vuelve al listado de proyectos  

---

### Entregables (consultar / volver) 
- [abrirProyecto](link) - El usuario regresa a la vista del proyecto relacionado  

---

### Investigadores (consultar) 
- [abrirInvestigador](link) - El usuario consulta el perfil de un investigador  
- [abrirInvestigadores](link) - El usuario vuelve al listado de investigadores  
- [abrirProyecto](link) - El usuario accede al proyecto asociado (si aplica)  
- [abrirPerfil](link) - El usuario retorna a su perfil desde esta vista  

---

## Casos de uso exclusivos del Coordinador

### Gestión avanzada de Publicaciones 
- [editarPublicacion](link) - El coordinador modifica una publicación de cualquier usuario  
- [eliminarPublicacion](link) - El coordinador elimina una publicación del sistema  

---

### Gestión avanzada de Proyectos 
- [crearProyecto](link) - El coordinador registra un nuevo proyecto  
- [editarProyecto](link) - El coordinador modifica la información de un proyecto  
- [eliminarProyecto](link) - El coordinador elimina un proyecto existente  
- [agregarInvestigador](link) - El coordinador añade un investigador a un proyecto  
- [eliminarInvestigador](link) - El coordinador retira un investigador de un proyecto  
- [crearEntregable](link) - El coordinador crea un nuevo entregable  
- [editarEntregable](link) - El coordinador modifica los datos de un entregable  
- [eliminarEntregable](link) - El coordinador elimina un entregable existente  

---

### Gestión de Investigadores 
- [crearInvestigador](link) - El coordinador registra un nuevo investigador en el sistema  

---

