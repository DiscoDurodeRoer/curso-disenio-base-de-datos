
[Video resolviendo todos los ejercicios](https://youtu.be/_OXqqOFKNb4)

# Ejercicio 1

Se desea diseñar una base de datos sobre la información de las reservas de una empresa dedicada al alquiler de automóviles teniendo en cuenta que:

Un determinado cliente puede tener en un momento dado hechas varias reservas.

De cada cliente se desea almacenar su DNI, nombre, dirección y teléfono. Ademas dos clientes se diferencian por un código unico.

Cada cliente puede ser avalado por otro cliente de la empresa.

Una reserva la realiza un único cliente pero puede involucrar a varios coches.

Es importante registrar la fecha de inicio y final de la reserva, el precio del alquiler de cada uno de los coches, los litros de gasolina en el deposito en el momento de realizar la reserva, el precio total de la reserva y un indicador de si el coche o los coches han sido entregados.

No se mantienen los datos de reservas anteriores.

Todo coche tiene siempre asignado un determinado garaje que no puede cambiar. De cada coche se requiere la matricula, el modelo, el color y la marca.

Cada reserva se realiza en una determinada agencia.

<details>
  <summary>Solución</summary>
  
  ![Descripción de la imagen](./ejercicio-1/solucion.png)
  
</details>

[Video resolviendo el ejercicio](https://youtu.be/NFb9eX9s3ZY)

# Ejercicio 2

La coordinadora nacional de ONGs desea mantener una base de datos de las asociaciones de este tipo que existen en nuestro pais. 

Para ello necesita almacenar información sobre cada asociación, los socios que las componen, los proyectos que realizan y los trabajadores de las mismas.

De las asociaciones se desea almacenar su CIF, denominación, dirección y provincia, su tipo (ecologista, integración, desarrollo, …), así como si esta declarada de utilidad publica por el Ministerio del Interior.

Cada asociación esta formada por socios de los que se precisa conocer su DNI, nombre, dirección, provincia, fecha de alta en la asociación, la cuota mensual con que colaboran y la aportación anual que realizan (que se obtendrá multiplicando la cuota mensual por los meses del año).

Los trabajadores de estas organizaciones pueden ser de dos tipos: asalariados y voluntarios.

Los asalariados son trabajadores que cobran un sueldo y ocupan cierto cargo en la asociación. Se desea almacenar la cantidad que éstos pagan a la seguridad social y el tanto por ciento de IRPF que se le descuenta.

Los voluntarios trabajan en la organización desinteresadamente, siendo preciso conocer su edad, profesión y las horas que dedican a la asociación a efectos de cálculo de estadisticas.

Cada trabajador se identifica por su DNI, tiene un nombre y fecha de ingreso.

Un socio no puede ser trabajador de la asociación.

Las asociaciones llevan a cabo proyectos a los que están asignados sus trabajadores. 

De cada proyecto se desea almacenar su número de identificación dentro de la asociación, en qué pais se lleva a cabo y en que zona de este, así como el objetivo que persigue y el numero de beneficiarios a los que afecta. 

Un proyecto se compone a su vez de subproyectos.

<details>
  <summary>Solución</summary>
  
  ![Descripción de la imagen](./ejercicio-2/solucion.png)
  
</details>

[Video resolviendo el ejercicio](https://youtu.be/3SFKqUnN4Cc)

# Ejercicio 3

Se pretende diseñar una base de datos sobre los servicios de urgencia de los hospitales.

En los servicios de urgencia trabajan empleados que pueden ser de dos tipos: conductores de ambulancias o personal sanitario. Un empleado no puede ser de los dos tipos a la vez y tiene que ser uno obligatoriamente.

De los empleados interesa saber: nombre, apellidos, DNI, dirección, teléfono, correo electrónico y estará identificado por un código de empleado.

De los conductores de ambulancias interesa saber ademas el tipo de carnet y lo que cobra cada hora de trabajo.

Del personal sanitario guardaremos su nivel y salario.

De cada hospital necesitamos almacenar: nombre del hospital, dirección, localidad, provincia, código postal, teléfono, categoría y especialidades que tiene. Cada hospital está identificado por un código de hospital.

Del personal sanitario interesa saber los hospitales en los que ha trabajado, las fechas de alta y de baja en cada hospital. Puede haber trabajado en muchos hospitales, como mínimo en uno. En un hospital trabajan muchos sanitarios. No puede haber hospitales sin personal sanitario.

Necesitamos registrar los viajes que realiza el conductor de ambulancia a los hospitales (puede no haber realizado ninguno). De cada viaje necesitamos saber: la fecha del viaje, población a la que ido a buscar al paciente, kilómetros realizados y n° de horas que ha tardado en realizarlo. Un conductor realizará muchos viajes a hospitales distintos.

Se necesitará registrar las guardias que hace cada personal sanitario en el hospital, se almacenará la fecha de al guardia, turno y n° de horas.

El personal sanitario formará parte de un grupo. Interesa saber el puesto que ocupa en ese grupo. Cada grupo tiene un código de grupo y nombre. Cada grupo puede estar formado por muchos sanitarios, como mínimo por uno.

Un conductor de ambulancia siempre conduce la misma ambulancia y una ambulancia siempre es conducida por el mismo conductor. Una ambulancia puede que no tenga asignado conductor. De al ambulancia sabemos su matrícula, tipo de ambulancia y instrumental médico que posee.

<details>
  <summary>Solución</summary>
  
  ![Descripción de la imagen](./ejercicio-3/solucion.png)
  
</details>

[Video resolviendo el ejercicio](https://youtu.be/Lwb89xS8Emo)
  
# Ejercicio 4

Lee atentamente la siguiente especificación de requisitos sobre la información a almacenar de una biblioteca para la gestión de las consultas a las enciclopedias por parte de los alumnos:
Dispone de enciclopedias formadas por varios tomos numerados ( I, II,III, IV,….). Esta numeración es igual para todos los tomos de las enciclopedias.

En la elaboración de las enciclopedias han participado varios autores y de cada enciclopedia almacenamos el ISBN, título, editorial y país de la editorial.

De cada tomo se almacena además del número de tomo y la primera y última palabra que contiene.

La consulta de los tomos se realiza a través de una tarjeta de acceso que incorpora, como se explica más adelante, el DNI del alumno, éste puede consultar más de una vez y con la misma tarjeta el mismo tomo, por lo que interesa guardar la fecha de consulta y durante cuánto tiempo lo tuvo cada vez.

Cada tarjeta tiene un tipo de acceso diferente a la biblioteca cada uno con un nº máximo de consultas permitidas y un precio.

Un alumno puede tener varias tarjetas de acceso pero de un tipo diferente cada una (por ello la entidad tarjeta tiene su clave primaria compuesta por dni+tipo_acceso), de cada alumno guardamos el DNI, nombre, ciclo formativo y nivel de estudios.

Hay que saber en qué armario se encuentra cada tomo. El armario se identifica por el número de pasillo y una letra, además se almacena también su capacidad.

En la biblioteca hay varios empleados (necesitamos almacenar algunos de sus datos personales como DNI, nombre y fecha de nacimiento). 

Unos se ocupan del mantenimiento de los armarios (de cada uno de estos tenemos que conocer qué tipo de función de mantenimiento tiene asignada), cuando realizan algún arreglo a un armario hay que anotar una breve descripción de lo que se le ha hecho y cuándo.

Otros empleados realizan solo tareas de gestión como la elaboración de las tarjetas de acceso (de estos interesa su titulación) y queremos conocer qué empleado ha sido el que ha elaborado cada una de las tarjetas.

<details>
  <summary>Solución</summary>
  
  ![Descripción de la imagen](./ejercicio-4/solucion.png)
  
</details>

[Video resolviendo el ejercicio](https://youtu.be/ZZ2dKyzIjic)

# Ejercicio 5

Se desea realizar una base de datos relacionada a la gestión de un torneo de ajedrez:

En el campeonato participan jugadores y árbitros, de ambos se requiere conocer el numero de asociado, nombre, dirección, teléfono de contacto y campeonatos en los que ha participado (como jugador o arbitro). 

De los jugadores se precisa ademas el nivel de juego en una escala de 1 a 10.

Ningún arbitro puede participar como jugador.

Los países envían al campeonato un conjunto de jugadores y árbitros, aunque no todos los países envían participantes. Todo jugador y arbitro es enviado por un único pais.

Un país puede ser representado por otro pais

Cada país se identifica por un numero correlativo según su orden alfabético e interesa conocer ademas su nombre, el numero de clubes de ajedrez existentes en el mismo.

Cada partido se identifica por un numero correlativo, la juegan dos jugadores y la arbitra un arbitro.
Interesa registrar las partidas que juega cada jugador y el color (blancas o negras) con el que juega.

Todo participante participa en al menos una partida.

Tanto jugadores como árbitros se alojan en hoteles en los que se desarrollan las partidas, se desea conocer en que hotel y en que fechas se ha alojado cada uno de los participantes.

Los participantes no tienen porque alojarse en un hotel.

De cada hotel se desea conocer el nombre, dirección y telefono.

El campeonato se desarrolla a lo largo de una serie de jornadas (año, mes, día).

Cada partida se celebra en una de las salas de los hoteles, se desea conocer el numero de entradas vendidas en la sala para cada partida.

De cada sala se desea conocer la capacidad y medios que dispone para facilitar la transmisión de los encuentros.

De cada partida, se registran todos los movimientos que la componen, la identificación de movimiento se establece en base a un numero de orden dentro de cada partida.

Para cada movimiento se guardan la jugada y un breve comentario de un experto

<details>
  <summary>Solución</summary>
  
  ![Descripción de la imagen](./ejercicio-5/solucion.png)
  
</details>

[Video resolviendo el ejercicio](https://youtu.be/z5orMNEL8p0)