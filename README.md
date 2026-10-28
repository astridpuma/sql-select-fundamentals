# sql-select-fundamentals

Consultas SQL para extraer información de una base de datos de ventas usando `SELECT`.
Ejercicio del curso de Data Analytics de Coderhouse.

## Objetivo
Practicar cómo obtener, filtrar y ordenar información de una base de datos relacional para responder preguntas de negocio.

##¿Por qué es mala práctica usar SELECT * en producción? Mencioná al menos dos razones concretas (rendimiento, mantenibilidad, seguridad).
a) En rendimiento es una mala práctica porque capaz de requieren solo los mails de una base que tenga 5000 registros. Significa que se van a multiplicar esos registros por la cantidad de campos trayendo mucha más información de la necesaria.
b) Porque no se especifica qué necesita la consulta, lo cual puede verse afectado si es que alguien modifica la base de datos, y el resultado de la consulta cambió, y la reportería también.
c) En seguridad, porque al traer toda la data se trae información sensible como datos personales.

##¿Por qué son importantes los alias para un stakeholder no técnico? Explicá con un ejemplo concreto cómo un alias transforma total_amount en algo que cualquier persona del área de finanzas puede interpretar directamente.
Porque es muy ambiguo el campo, puede ser que el monto total sea con impuestos, por lo que si no se detalla, el área de finanzas puede entender que se trata del monto sin impuestos y adicionarlo al momento de facturarle al cliente si compró algo. Por eso se utilizan los alias para que las columnas puedan traducirse al idioma del negocio. 
