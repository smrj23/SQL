![[Diagrama.png]]
Para poder crear una base de datos sobre escuela, mi principal enfoque fue sobre el alumno y lo que conlleva su ambiente. Se tiene que ver de la manera mas abstracta posible para desarrollar una arquitectura de base de datos la cual no tenga que mayores cambios a futuro. 

Es por esto que se divide de la manera absoluta, creando las siguientes tablas:

* Apoderado del estudiante: Consta de un mail, con su nombre y apellido para poder identificar. su clave primaria es el id del apoderado.

* Estudiante: Cuenta con su nombre y apellido para poder identificar, la fecha en que admite, su mail y clave para sus ramificaciones. Su clave primaria es id del estudiante.

* Asistencia: La asistencia es punto importante dentro del colegio, se crea la variable asistencia como booleana para saber si asiste o no, junto con la fecha. Esta depende del id del estudiante. 

* Resultados: Este quiere decir si paso la materia cursada, es por lo mismo que la columna resultado es booleana para saber si es un si o no, depende del alumno y su materia.

* Materia: Cuando hablamos de materia queremos decir si es matematicas, biologia, etc. Esta depende del curso, y su clave primaria es la id de la materia.

* Curso: Cuando hablamos de curso queremos decir si esta cursando octavo, primero medio, etc. Se puede utilizar una lista de cursos posibles para limitar la informacion si es necesario, pero en este caso solo se crea la columna nombre para identificarse. 

* Sala de clase: Depende del profesor y de la materia. Tenemos la informacion del anno en que se produce.

* Estudiante sala: Depende del estudiante y la sala de clases.

* Profesores: Tiene un mail propio, cuenta con la admision, nombre y apellido. Su clave primaria es su id.

Finalmente para poder ver codigo de la base de datos vease https://github.com/smrj23/SQL/blob/main/escuela. 

Datos importantes es el orden con cual se crea las tablas, porque si creamos una tabla que dependa de otra y esta no existe no se podra generar. Mi consejo querido lector para mejorar en la arquitectura de base de datos es crear mas y poder crear este tipo de relaciones sin mayores problemas.


 

  