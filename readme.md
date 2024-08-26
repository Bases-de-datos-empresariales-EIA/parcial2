1. Construcción de un diagrama Entidad-Relación (40%):

Construya el diagrama Entidad-Relación basado en la siguiente descripción de negocio.

Descripción del negocio:

Una academia de música llamada "Notas y Acordes" ofrece clases de diferentes instrumentos musicales. La academia tiene un catálogo de cursos, cada uno con un nombre, descripción, nivel de dificultad (básico, intermedio, avanzado) y precio. Los estudiantes pueden inscribirse en uno o más cursos. Cada estudiante tiene un nombre, correo electrónico y teléfono. La academia también lleva un registro de los instructores, quienes imparten uno o varios cursos. Cada instructor tiene un nombre, especialidad, y años de experiencia.

Consideraciones:

Un estudiante puede inscribirse en múltiples cursos.
Cada inscripción está asociada a un solo curso y un solo estudiante.
Un curso puede ser impartido por múltiples instructores.
Un instructor puede impartir múltiples cursos.

Calificación:

- Las relaciones están bien mapeadas (10%)
- El diagrama cumple con el estándar visto en clase (15%)
- El diagrama cumple con la descripción del negocio (15%)

---

2. Construya el script de creación de tablas en SQL para el siguiente diagrama E-R (10%):

![Diagrama E-R](./media/punto-2.png)

---

3. Considere el siguiente diagrama E-R (50%):

![Diagrama E-R](./media/punto-3.png)

La base de datos estructurada en este diagrama ER está diseñada para gestionar la información operacional de una empresa que maneja relaciones contractuales con diversos clientes y registra actividades de empleados a través de reportes de horas. La estructura del esquema facilita el seguimiento y la administración eficiente de los siguientes componentes clave del negocio:

Usuarios (Usuarios): Representa a los empleados de la empresa. Cada usuario tiene un registro único identificado por un ID, y el esquema permite almacenar nombres y apellidos opcionales. Los usuarios son responsables de crear reportes que documentan las horas trabajadas en diversos proyectos o contratos.

Clientes (Clientes): Esta entidad almacena información sobre los clientes de la empresa. Cada cliente tiene un ID único y campos opcionales para el NIT y el nombre. Los clientes son fundamentales para el negocio, ya que mantienen contratos activos que generan ingresos.

Contratos (Contratos): Los contratos son acuerdos comerciales entre la empresa y sus clientes. Cada contrato, identificado también por un ID único, tiene asociado un nombre y valores de venta y costo que ayudan a evaluar la rentabilidad de cada acuerdo. Cada contrato está vinculado a un cliente específico y puede tener varios reportes asociados.

Reportes (Reportes): Los reportes son registros detallados de las actividades realizadas por los usuarios, donde se documentan las horas dedicadas y las fechas específicas de trabajo. Estos reportes están vinculados tanto a los contratos bajo los cuales se realizan las actividades como a los usuarios que las ejecutan.

Responda las preguntas listadas a continuación. Cada pregunta tiene un valor del 10%, que se reparte en dos mitades:

- Respuesta correcta: 5%
- Query: 5%

Preguntas:

- Escriba un query que calcule el total de ingresos generados por cada cliente a través de sus contratos. Deberá sumar el valor de las ventas de todos los contratos asociados a cada cliente y mostrar el nombre del cliente junto con los ingresos totales. Responda:
  - ¿Cuál es el top 3 de clientes que han generado más ingresos? ¿Cuánto ingreso generó cada uno de ellos? (10%)
- Formule un query que calcule el total de horas trabajadas reportadas por cada usuario durante Julio del 2024. Los resultados deben incluir el nombre, apellido y total de horas reportadas de cada usuario.
  - ¿Cuál es el top 3 de usuarios con más horas reportadas en Julio del 2024? ¿Cuántas horas reportó cada uno de ellos? (10%)
- Cree un query que calcule el total de horas reportadas en cada contrato durante el año en curso. Los resultados deben incluir el nombre del contrato y el número total de reportes.
  - ¿Cuáles son los 3 contratos con más horas reportadas durante el 2024? ¿Cuántas horas hay reportadas en cada uno de ellos? (10%)
- Formule un query que muestre el total de las horas trabajadas por mes y año durante el 2023.
  - ¿Cuál fue el mes que más se trabajó en el 2023? ¿Cuántas horas se trabajaron en ese mes? (10%)
- Construya un query que calcule el reporte de horas más grande generado por cada usuario.
  - ¿Cuáles son los dos usuarios con los reportes individuales más grandes y cuántas horas reportó cada uno? (10%)

---
