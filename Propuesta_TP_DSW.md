# Propuesta TP DSW

## Grupo

### Integrantes

Oliva, Laureano Ivan        48501

Salvía, Camila                    49373

Zallocco, Emilio                50194

### Repositorios

* [fullstack](https://github.com/camila-salvia/pagina-universitaria-dsw)
  
  ## Tema
  
  ### Descripción
  
  El software desarrollado permitirá que los alumnos de la facultad puedan visualizar en un mismo lugar todo lo necesario de su estado académico, así como por ejemplo, sus notas, cursos en los que está inscripto o exámenes. También permite a los profesores hacer un seguimiento académico de sus alumnos.
  
  ### Modelo
  ```mermaid
  classDiagram
    Clase --* Persona
    class Clase{
        Pagina Estatica
        Tabla De Notas
    }
    class Persona{
        Usuario
        Contrasena
    }
  ```
  
  
  # Funciones Principales
  
  Del alumno
  - Mostrar los cursos en los que está inscripto.
  
  - Inscribirse a un nuevo curso.
  
  - Anotarse a un examen.
  
  - Solicitar una clase de consulta de un curso determinado.
  
  - Permitir a los alumnos ver solamente sus notas.
  
  Del profesor
  
  - Cargar las notas de los alumnos.
  
  - Permitir a los profesores hacer el seguimiento de las notas de cada alumno en el curso a través de una tabla.
  
  - Subir información sobre el curso, así como apuntes o libros.
  
  - Agendar una clase de consulta.
  
  - Añadir una fecha de examen.
  
  ## Necesidades de Implementación
  
  - Logueo de Usuarios.
  
  - Páginas estáticas de cada curso.
  
  - Página Dinámica que se actualiza segun quien es el usuario.
  
  - Tabla de Notas x curso para seguimiento de las notas por el profesor.
    
    
  
  ## Alcance Funcional
  
  ### Alcance Mínimo
  
  *Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 
  Regularidad:
  
  | Req                         | Detalle                                                                                                                                                                                                                                                                                                                           |
  |:--------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  | CRUD simple                 | 1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad                                                                                                                                                                                                                                                                  |
  | CRUD dependiente            | 1. CRUD Habitación {depende de} CRUD Tipo Habitacion<br>2. CRUD Cliente {depende de} CRUD Localidad                                                                                                                                                                                                                               |
  | Listado<br>+<br>detalle     | 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente |
  | CUU/Epic                    | 1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva                                                                                                                                                                                                                                              |
  | Adicionales para Aprobación |                                                                                                                                                                                                                                                                                                                                   |
  | Req                         | Detalle                                                                                                                                                                                                                                                                                                                           |
  | :-                          | :-                                                                                                                                                                                                                                                                                                                                |
  | CRUD                        | 1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente                                                                                                                                                                                |
  | CUU/Epic                    | 1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios                                                                                                                                                                             |
  
  ### Alcance Adicional Voluntario
  
  *Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.
  
  | Req      | Detalle                                                                                                                                                                                                             |
  |:-------- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  | Listados | 1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes |
  | CUU/Epic | 1. Consumir servicios<br>2. Cancelación de reserva                                                                                                                                                                  |
  | Otros    | 1. Envío de recordatorio de reserva por email                                                                                                                                                                       |
