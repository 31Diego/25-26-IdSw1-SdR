# 🧩 Detalle del Prototipo: Casos de Uso (CDU)

## 🧑‍💼 Casos de Uso del Coordinador

### 🔐 Gestión de sesión y perfil

#### [iniciarSesion](iniciarSesion)
- Formulario con campos **Correo** y **Contraseña**.
- Botón **Iniciar sesión**.
- Si falla, muestra error.

#### [cerrarSesion](cerrarSesion)
- Botón en menú superior.
- Cierra sesión y redirige a login.

#### [denegarInicioSesion](denegarInicioSesion)
- Alerta roja: “Credenciales inválidas”.
- Formulario permanece visible.

#### [abrirOpcionesPerfil](abrirOpcionesPerfil)
- Panel con datos personales editables: nombre, CV, área, sede.
- Botón “Guardar”.

#### [editarPerfil](editarPerfil)
- Mismo panel editable.
- Guarda cambios al enviar.

#### [eliminarPerfil](eliminarPerfil)
- Confirmación modal: “¿Eliminar tu perfil?”.
- Botón “Eliminar”.

#### [abrirOpcionesCargaTrabajo](abrirOpcionesCargaTrabajo)
- Muestra carga docente (h/16), proyectos activos y total.
- Permite ajustar manualmente.

#### [editarCargaTrabajo](editarCargaTrabajo)
- Formulario para modificar horas asignadas.
- Validación si supera 16h.

---

### 📊 Dashboard

#### [verAccionesRapidas](verAccionesRapidas)
- Botones: Nuevo proyecto, Crear propuesta, Ver investigadores, Ver convocatorias.

#### [verIndicadores](verIndicadores)
- Gráficos:
  - Propuestas presentadas
  - Proyectos financiados
  - Distribución por sede

#### [gestionarAlertas](gestionarAlertas)
- Lista de alertas:
  - “Entregable vence en 3 días”
  - “Proyecto sin responsable”
- Botón “Marcar como leída”.

---

### 📁 Gestión de proyectos

#### [abrirProyectos](abrirProyectos)
- Tabla: Título, Estado, Financiador, Fechas.
- Filtros por estado.

#### [crearProyecto](crearProyecto)
- Formulario: título, descripción, equipo, presupuesto.
- Botón “Crear”.

#### [nuevoProyecto](nuevoProyecto)
- Igual que crearProyecto(), pero prellenado desde propuesta aceptada.

#### [abrirProyecto](abrirProyecto)
- Vista detallada: objetivos, equipo, entregables, presupuesto, estado.

#### [editarProyecto](editarProyecto)
- Todos los campos editables.
- Botón “Guardar cambios”.

#### [eliminarProyecto](eliminarProyecto)
- Confirmación: “¿Eliminar este proyecto? No se puede deshacer”.
- Botón “Sí, eliminar”.

#### [agregarInvestigador](agregarInvestigador)
- Selector múltiple de investigadores con carga (<16h).
- Botón “Añadir”.

#### [eliminarInvestigador](eliminarInvestigador)
- Ícono “X” junto al investigador.
- Confirmación modal.

---

### 📦 Gestión de entregables

#### [abrirEntregables](abrirEntregables)
- Lista: título, fecha límite, estado.
- Botón “Ver”.

#### [crearEntregable](crearEntregable)
- Formulario: título, descripción, fecha límite, responsable.
- Botón “Crear”.

#### [editarEntregable](editarEntregable)
- Edición completa.
- Botón “Actualizar”.

#### [eliminarEntregable](eliminarEntregable)
- Confirmación modal.
- Botón “Eliminar”.

---

### 👩‍🔬 Gestión de investigadores

#### [abrirInvestigadores](abrirInvestigadores)
- Lista: nombre, sede, área, carga (X/16).
- Buscador y filtros.

#### [crearInvestigador](crearInvestigador)
- Formulario: nombre, correo, perfil, sede, CV.
- Botón “Registrar”.

#### [abrirInvestigador](abrirInvestigador)
- Perfil completo: datos, proyectos, carga, compensaciones.

#### [asignarAProyecto](asignarAProyecto)
- Selector de proyectos.
- Botón “Asignar”.

#### [gestionarCompensacion](gestionarCompensacion)
- Modal:
  - Reducir horas docentes
  - Recibir pago
- Botón “Enviar”.

---

### 📢 Convocatorias

#### [verConvocatorias](verConvocatorias)
- Lista: título, financiador, fecha límite, estado.
- Botón “Ver detalles”.

#### [abrirConvocatoria](abrirConvocatoria)
- Detalles: requisitos, importe, duración, documentos.

#### [crearConvocatoria](crearConvocatoria)
- Formulario completo.
- Botón “Registrar”.

#### [editarConvocatoria](editarConvocatoria)
- Edición total.
- Botón “Guardar”.

#### [eliminarConvocatoria](eliminarConvocatoria)
- Confirmación modal.
- Botón “Sí, eliminar”.

#### [generarPropuesta](generarPropuesta)
- Botón “Crear propuesta vinculada”.

---

### 📝 Propuestas

#### [crearPropuesta](crearPropuesta)
- Formulario: título, resumen, equipo, presupuesto.
- Vinculada a convocatoria.

#### [abrirPropuesta](abrirPropuesta)
- Vista detallada: estado, evaluación, documentos.

#### [editarPropuesta](editarPropuesta)
- Editable solo antes de presentar.

#### [eliminarPropuesta](eliminarPropuesta)
- Solo si está en “Borrador”.

#### [convertirEnProyecto](convertirEnProyecto)
- Botón “Convertir en proyecto”.

---

### 🗣️ Publicaciones

#### [abrirPublicaciones](abrirPublicaciones)
- Muro general.  
- Botón “Responder”.

#### [abrirPublicacion](abrirPublicacion)
- Publicación completa con comentarios.

#### [responderPublicacion](responderPublicacion)
- Campo de texto + botón “Enviar”.

#### [editarPublicacion](editarPublicacion)
- Solo propias o del coordinador.

#### [eliminarPublicacion](eliminarPublicacion)
- Ícono 🗑️ + confirmación.

#### [abrirMisPublicaciones](abrirMisPublicaciones)
- Lista propia.

#### [abrirMiPublicacion](abrirMiPublicacion)
- Vista individual.

#### [crearPublicacion](crearPublicacion)
- Formulario: título y cuerpo.  
- Botón “Publicar”.

---

# 👩‍🔬 Casos de Uso del Investigador

### 🔐 Gestión de sesión y perfil
*(Igual que coordinador)*

#### [iniciarSesion](iniciarSesion)
#### [cerrarSesion](cerrarSesion)
#### [denegarInicioSesion](denegarInicioSesion)

#### [abrirOpcionesPerfil](abrirOpcionesPerfil)
- Panel editable.

#### [editarPerfil](editarPerfil)
- Guarda cambios.

---

### ⏱️ Carga de trabajo

#### [verMiCargaTrabajo](verMiCargaTrabajo)
- Horas docentes, proyectos y total.
- Botón “Solicitar compensación”.

#### [solicitarCompensacion](solicitarCompensacion)
- Modal:
  - Reducir horas
  - Recibir pago  
- Botón “Enviar solicitud”.

---

### 📁 Proyectos

#### [verMisProyectos](verMisProyectos)
- Proyectos donde participa.
- Próximos entregables.

#### [abrirProyecto](abrirProyecto)
- Solo lectura.

#### [subirEntregable](subirEntregable)
- Formulario + archivo.  
- Botón “Subir”.

---

### 📢 Convocatorias y propuestas

#### [verConvocatorias](verConvocatorias)
- Convocatorias abiertas.

#### [verConvocatoria](verConvocatoria)
- Detalles completos.

#### [crearPropuesta](crearPropuesta)
- Desde convocatoria.

#### [abrirPropuesta](abrirPropuesta)
- Vista propia.

#### [editarPropuesta](editarPropuesta)
- Solo en borrador.

#### [eliminarPropuesta](eliminarPropuesta)
- Confirmación.  
- Solo en borrador.

---

### 🗣️ Publicaciones

#### [abrirPublicaciones](abrirPublicaciones)
#### [abrirPublicacion](abrirPublicacion)
#### [responderPublicacion](responderPublicacion)
#### [abrirMisPublicaciones](abrirMisPublicaciones)
#### [abrirMiPublicacion](abrirMiPublicacion)
#### [crearPublicacion](crearPublicacion)
#### [editarPublicacion](editarPublicacion)
#### [eliminarPublicacion](eliminarPublicacion)
