# Modelo del dominio Gestor Investigadores y Proyectos Funiber (GIPF)

## Objetivo

#### El objetivo de este proyecto es diseñar un solo sistema en donde:
#### 1. Estén registradas las diferentes entidades de la red de Funiber (investigador, coordinador, etc), los cuales podrán interactuar entre ellos.
#### 2. Se pueda llevar una gestión de los proyectos asociados con los investigadores, en donde entre otras cosas se podrán revisar los entregables de un proyecto.




## Vocabulario del proyecto

#### En base a nuestra primera reunión definimos los términos clave del proyecto y los explicamos, a continuación los términos mas importantes del [vocabulario](https://github.com/31Diego/25-26-IdSw1-SdR/blob/Diego/documentaci%C3%B3n/ModeloDelDominio/Documentos/Vocabulario.md)

---

###  Estados de un proyecto

| **Término** | **Definición** | **Notas / Ejemplo** |
|--------------|----------------|----------------------|
| **Entidad convocante** | Organización o institución que emite una convocatoria. | Puede ser la Unión Europea, el Ministerio de Ciencia, el Gobierno de Cantabria, etc. |
| **Convocatoria** | Anuncio oficial de una oportunidad de financiación o participación en un proyecto de investigación. | Ejemplo: “Convocatoria Horizonte Europa 2025”. |
| **Propuesta** | Siguiente fase de una convocatoria, en donde se concretan los detalles de la misma | Ejemplo: Investigación sobre enfermedad rara.|
| **Proyecto** | Última fase de una convocatoria, en donde se tienen unos objetivos, un grupo de investigadores/docentes, una fecha de entrega y una documentación del mismo| ----- |

---

###  Usuarios y Roles

| **Término** | **Definición** | **Notas / Ejemplo** |
|--------------|----------------|----------------------|
| **Investigador / Docente** | Usuario registrado que busca, participa o coordina proyectos de investigación. | Incluye personal académico afiliado a FUNIBER. |
| **Perfil de investigador** | Conjunto de datos que describen la especialización, intereses, experiencia y criterios de elegibilidad del usuario. | Se utiliza para filtrar y recomendar convocatorias. |
| **Coordinador** | Rol o proceso encargado de revisar que la información (convocatorias, proyectos, documentación) sea correcta antes de su publicación. | Puede ser un rol administrativo dentro del sistema. |
| **Antena** | Rol o proceso encargado de estar al tanto de nuevas convocatorias | Puede ser un rol administrativo dentro del sistema (coordinador y antena están en el mismo nivel de permisos dentro del sistema)|

---



#### Una vez definido el vocabulario nos damos cuenta de que nuestro sistema se divide en dos subsistemas, uno relacionado con los investigadores/docentes y otro relacionado con los proyectos.


## Diagramas de clases

#### En el caso de los investigadores/docentes se modela como estos pueden interactuar entre si, estar participando en un proyecto o ser reclutados por un coordinador para participar en uno, etc. 

#### En el caso del subsistema de los proyectos se modela las diferentes fases del mismo, como pasa de convocatoria a propuesta y en ultima instancia a proyecto, tambien se representa lo que tiene asociado un proyecto como los entregables o el estado del mismo.



<div align=center>

|![](/documentación/ModeloDelDominio/Imagenes/Clases/ClasesProyecto.svg)|![](/documentación/ModeloDelDominio/Imagenes/Clases/ClasesRed.svg)|
|:-:|:-:|
|**Diagrama de clases de los proyectos**| **Diagrama de clases de la red de investigadores**|
</div>


#### Si nos damos cuenta, ambos diagramas tienen muchas entidades en común, por lo que en un principio los podriamos fusionar, quedando como resultado este diagrama.


<div align=center>

|![](/documentación/ModeloDelDominio/Imagenes/Clases/ClasesProyectoRed.svg)|
|:-:|
|**Diagrama de clases de los proyectos + red de investigadores**| 
</div>

#### Sin embargo para realizar los diagramas de estados utilizaremos los diagramas que indiquen el contexto de la gestión de los proyectos o la red de investigadores, no el que fusiona a los dos.


## Diagramas de estados

#### En los diagramas de estado se ha modelado el ciclo de vida de las entidades investigador/docente y proyecto, las cuales son las principales en sus diagramas de clases.



<div align=center>

|![](/documentación/ModeloDelDominio/Imagenes/Estados/EstadoProyecto.svg)|![](/documentación/ModeloDelDominio/Imagenes/Estados/EstadoInvestigador.svg)|
|:-:|:-:|
|**Diagrama de estados del ciclo de vida de un proyecto**| **Diagrama de estados del ciclo de vida de un investigador**|
</div>



