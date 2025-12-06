##  Detalle y Prototipado del Caso de Uso: `crearProyecto()`

### Información del Artefacto

| Atributo | Valor |
| :--- | :--- |
| **Proyecto** | Gestor Investigadores y Proyectos Funiber (GIPF) |
| **Fase RUP** | Elaboración |
| **Disciplina** | Requisitos |

### Propósito

Especificación detallada del caso de uso **crearProyecto()** mediante diagrama de estado, mostrando la conversación completa entre el **Coordinador** y el Sistema para el proceso de registro de un nuevo proyecto de investigación.

### Información del Caso de Uso

| Atributo | Valor |
| :--- | :--- |
| **Nombre** | `crearProyecto()` |
| **Actor primario** | Coordinador |
| **Objetivo** | Registrar un nuevo proyecto de investigación en el sistema. |
| **Tipo** | Primario, esencial |
| **Nivel** | Objetivo de usuario |
| **Precondición** | El Coordinador está autenticado y en el estado `PROYECTOS_ABIERTOS`. |
| **Postcondición exitosa** | El nuevo proyecto se registra y el sistema permanece en `PROYECTOS_ABIERTOS` con la lista actualizada. |
| **Postcondición de fallo** | El proyecto no se registra (ej. por datos inválidos) y el sistema permanece en `PROYECTOS_ABIERTOS` (o en la pantalla de entrada de datos con mensaje de error). |

---

## Diagrama de Especificación

Aquí se visualiza la conversación completa entre el Coordinador y el Sistema.

![Diagrama de Especificación](diagramaEstadoCrearProyecto.png)

## Prototipo de Interfaz

### Propósito del Prototipo

**Objetivo:** Obtener validación de la especificación y la usabilidad de la interfaz de entrada de datos clave antes de la inversión en desarrollo.

### Wireframes

#### Pantalla 1: Formulario de Creación de Proyecto (Estado Normal)

**Estado:** SolicitandoDatosProyecto → ProporcionandoDatosProyecto

**Correspondencia con especificación:**
* Actor "crea proyecto" (transición previa).
* Sistema "permite ingresar datos" (se presenta la interfaz).

| Elemento | Tipo de Campo | Ejemplo/Nota |
| :--- | :--- | :--- |
| **Título del Proyecto** | Texto Obligatorio | "Investigación sobre IA en salud" |
| **Descripción** | Área de Texto | Resumen del objetivo y alcance. |
| **Fecha de Inicio** | Selector de Fecha | Por defecto: Fecha actual. |
| **Fecha de Fin Estimada** | Selector de Fecha | Fecha límite del proyecto. |
| **Botón de Acción** | Primario | "Crear Proyecto" |

#### Pantalla 2: Formulario de Creación de Proyecto (Estado de Error)

**Estado:** Choice point → regreso a SolicitandoDatosProyecto (por validación fallida)

**Correspondencia con especificación:**
* Choice point evalúa: "usuario:datos inválidos" (ej. Título vacío).
* Sistema presenta mismo diálogo + mensaje de error.

**Mensaje de Error:** "Error: El Título del Proyecto es obligatorio. Por favor, revísalo."

### Validaciones del Wireframe

* ¿Los campos clave (título, fechas) son suficientes para registrar un proyecto inicial?
* ¿El mensaje de error indica claramente al Coordinador qué debe corregir?
* ¿La terminología utilizada (e.g., "Crear Proyecto") es consistente con el dominio?
* ¿La especificación carece de algún dato obligatorio que el wireframe revela (ej. ¿se necesita un campo de "Presupuesto"?)?

---

## Conversación Detallada

### Flujo Principal (Éxito)

| Actor | Acción | Sistema | Respuesta/Resultado |
| :--- | :--- | :--- | :--- |
| **Coordinador** | selecciona la opción **"Crear Proyecto"** | **Sistema** | Muestra el formulario de entrada de datos (Título, Descripción, Fechas). |
| **Coordinador** | **introduce** Título, Descripción y Fechas, luego **confirma** la creación. | **usuario:datos válidos** | Se registra el nuevo proyecto. Se muestra mensaje de confirmación y regresa a la lista de proyectos (`PROYECTOS_ABIERTOS`). |

### Flujo Alternativo (Error de Datos)

| Actor | Acción | Sistema | Respuesta/Resultado |
| :--- | :--- | :--- | :--- |
| **Coordinador** | selecciona la opción **"Crear Proyecto"** | **Sistema** | Muestra el formulario de entrada de datos (Título, Descripción, Fechas). |
| **Coordinador** | **introduce** datos, dejando el campo *Título* vacío, y **confirma**. | **usuario:datos inválidos** | **Sistema** presenta el formulario nuevamente con un mensaje de error que indica que el Título es obligatorio. |

### Estados Internos del Caso de Uso

| Estado | Descripción | Responsabilidad |
| :--- | :--- | :--- |
| **SolicitandoDatosProyecto** | Estado donde el Coordinador necesita proporcionar la información del nuevo proyecto. | Sistema debe presentar el formulario. |
| **ProporcionandoDatosProyecto** | El Coordinador está rellenando o ha rellenado los campos. | Sistema recibe la entrada de datos. |
| **PuntoDeDecision** | Evaluación de los datos introducidos para verificar su validez (campos obligatorios, formatos). | Sistema determina la validez de los datos. |

### Validaciones del Sistema

| Validación | Criterio | Resultado |
| :--- | :--- | :--- |
| **Datos de Proyecto Válidos** | Campos obligatorios completados y con formato correcto (ej. Título no vacío, Fechas coherentes). | Se guarda el proyecto. Transición a `RegistroExitoso`. |
| **Datos de Proyecto Inválidos** | Falta un campo obligatorio o un formato es incorrecto. | El proyecto no se guarda. Transición a `RegistroFallido` y regreso a `SolicitandoDatosProyecto` con error. |

---

## Conexión con Diagrama de Contexto

Este caso de uso corresponde a la transición:
$$\text{PROYECTOS\_ABIERTOS} \xrightarrow{\text{crearProyecto()}} \text{PROYECTO\_ABIERTO}$$
(Nota: En tu diagrama, `crearProyecto()` lleva de `PROYECTOS_ABIERTOS` a `PROYECTO_ABIERTO`. Mi detalle finaliza volviendo a la lista, lo que es un flujo común después de la creación, asumo que `PROYECTO_ABIERTO` es la vista detallada del proyecto recién creado o que se vuelve a la lista `PROYECTOS_ABIERTOS`).

### Características Metodológicas

| Característica | Detalle |
| :--- | :--- |
| **Separación de Responsabilidades** | **Actor** inicia la acción e introduce los datos. **Sistema** permite y valida. |
| **Ausencia de Detalles de Implementación** | No se especifica la tecnología de la interfaz, el tipo de base de datos, o la lógica de *guardado* específica. |
| **Conversación Atómica** | Representa una conversación completa: inicio, entrada de datos, y terminación en éxito/fallo. |
| **Transformación del Actor** | **No aplica directamente**; el actor permanece como **Coordinador** con los mismos permisos. |
