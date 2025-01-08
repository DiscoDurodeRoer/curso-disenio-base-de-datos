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
  
  ![Descripción de la imagen](./solucion.png)
  
</details>

[Video resolviendo el ejercicio](https://youtu.be/Lwb89xS8Emo)