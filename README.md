# Visualizacion y storytelling

## Dashboard 2: visualización y documentación para narrar a un equipo de trabajo


![image](https://github.com/rubyal/Visualizaci-n-y-storytelling/assets/88467602/4598bb0a-b80c-4915-b780-494108506702)

## Variables en la Base de Datos Original

### Timestamp
Tipo de variable: fecha y hora

Descripción: Fecha y hora exacta en que se completó la encuesta.
### How old are you?
Tipo de variable: Texto.

Descripción: Rango de edad del encuestado.
### What industry do you work in?
Tipo de variable: Texto.

Descripción: Industria en la que trabaja el encuestado.

### Job title
Tipo de variable: Texto.

Descripción: Título del puesto de trabajo del encuestado.

### If your job title needs additional context, please clarify here:
Tipo de variable: Texto.

Descripción: Contexto adicional sobre el título del puesto de trabajo

### What is your annual salary? (You'll indicate the currency in a later question. If you are part-time or hourly, please enter an annualized equivalent -- what you would earn if you worked the job 40 hours a week, 52 weeks a year.)
Tipo de variable: Número.

Descripción: Salario anual del encuestado (sin especificar la moneda).

### How much additional monetary compensation do you get, if any (for example, bonuses or overtime in an average year)? Please only include monetary compensation here, not the value of benefits.
Tipo de variable: Texto.

Descripción:
### Please indicate the currency
Tipo de variable: Texto.

Descripción: Moneda en la que se paga el salario anual.

### If "Other," please indicate the currency here:
Tipo de variable: Texto.

Descripción: En el caso de haber otra moneda en la que se paga el salario anual.

### If your income needs additional context, please provide it here:
Tipo de variable: Texto.

Descripción: Contexto adicional respecto a los ingresos.

### What country do you work in?
Tipo de variable: Texto.

Descripción: País donde trabaja el encuestado.

### If you're in the U.S., what state do you work in?
Tipo de variable: Texto.

Descripción: Si el encuestado se en Estados Unidos, indica en qué estado trabaja.

### What city do you work in?
Tipo de variable: Texto.

Descripción: Ciudad donde trabaja el encuestado.
### How many years of professional work experience do you have overall?
Tipo de variable: Texto.

Descripción: Años totales de experiencia laboral profesional del encuestado.
### How many years of professional work experience do you have in your field?
Tipo de variable: Texto.

Descripción: Años de experiencia laboral profesional en su campo actual del encuestado.
### What is your highest level of education completed?
Tipo de variable: Texto.

Descripción: Nivel más alto de educación completado por el encuestado.
### What is your gender?
Tipo de variable: Texto.

Descripción: Género con el que se identifica el encuestado.
### What is your race? (Choose all that apply.)
Tipo de variable: Texto.

Descripción: Raza(s) con la(s) que se identifica el encuestado.

## Variables luego de modeladas
DateTime: Fecha y hora exacta en que se completó la encuesta. (Tipo de dato: Fecha y Hora)

Age: Rango de edad del encuestado. (Tipo de dato: Texto)

Industry: Industria en la que trabaja el encuestado. (Tipo de dato: Texto)

JobTitle: Título del puesto de trabajo del encuestado. (Tipo de dato: Texto)

JobContext: Contexto adicional sobre el título del puesto de trabajo. (Tipo de dato: Texto)

AnnualSalary: Salario anual del encuestado. (Tipo de dato: Número)

AdditionalCompensation: Bonificaciones u horas extras en un año promedio. (Tipo de dato: Número)

Currency: Moneda en la que se paga el salario anual. (Tipo de dato: Texto)

OtherCurrency: En el caso de haber otra moneda en la que se paga el salario anual. (Tipo de dato: Texto)

IncomeContext: Contexto adicional respecto a los ingresos. (Tipo de dato: Texto)

Country: País donde trabaja el encuestado. (Tipo de dato: Texto)

State_USA: Si el encuestado se encuentra en Estados Unidos, indica en qué estado trabaja. (Tipo de dato: Texto)

City: Ciudad donde trabaja el encuestado. (Tipo de dato: Texto)

TotalExperience: Años totales de experiencia laboral profesional del encuestado. (Tipo de dato: Texto)

FieldExperience: Años de experiencia laboral profesional en su campo actual del encuestado. (Tipo de dato: Texto)

Education: Nivel más alto de educación completado por el encuestado. (Tipo de dato: Texto)

Gender: Género con el que se identifica el encuestado. (Tipo de dato: Texto)

Race: Raza(s) con la(s) que se identifica el encuestado. (Tipo de dato: Texto)


## Guía paso a paso: Actualización de Datos y Modelado para Dashboard 
Aquí hay un paso a paso detallado para actualizar los datos y aplicar el modelado en un dashboard:

#### 1.	Acceso a la origen de datos (Excel: Ask A Manager Salary Survey 2021 (Responses) (1)):

Accede al origen de datos de forma local, en nube o sitio compartido

Verifica que tengas los permisos necesarios para realizar cambios en el archivo.

Actualización de los Datos:

#### 2.	Identifica la tabla o tablas en la base de datos que contienen los datos necesarios para el dashboard.

Si hay nuevos datos disponibles, asegúrate de que estén correctamente formateados y listos para ser cargados en la base de datos.

Asegúrate de que los nuevos datos se integren correctamente con los datos existentes.

#### 3.	Creación de Nuevos Campos:

Revisa los requisitos del modelo de datos y determina si es necesario agregar nuevos campos a las tablas existentes.

Ir a la vista de Datos: Cambia a la vista de Datos seleccionando el icono correspondiente en la barra lateral izquierda.

Seleccionar tabla: Haz clic en la tabla a la que quieres agregar la columna.

Agregar nueva columna: En la cinta de opciones, haz clic en "Nueva columna". Esto abrirá el editor de fórmulas en la parte superior de la ventana.

Escribir la fórmula DAX: En el editor de fórmulas, escribe la fórmula DAX para tu nueva columna. DAX (Data Analysis Expressions) es el lenguaje de fórmulas utilizado en el 
modelo de datos de Power BI.

Nombrar la columna: Asegúrate de darle un nombre descriptivo a tu nueva columna en la fórmula, antes del signo igual (=).

Presionar Enter: Una vez escrita tu fórmula y nombrada tu columna, presiona Enter para crear la columna.

#### 4. Procedimientos de Limpieza de Datos:
Opción 1: Utiliza scripts para ejecutar los procedimientos de limpieza de datos en las tablas correspondientes.

Opción 2: 
Abrir Editor de Power Query: Una vez que tus datos están cargados, ve a la vista de "Datos" o "Modelo" y haz clic en "Transformar datos" para abrir el Editor de Power Query.

Seleccionar la columna: En el Editor de Power Query, navega hasta la tabla y la columna donde deseas reemplazar valores.

Reemplazar valores: Haz clic derecho en el encabezado de la columna y elige "Reemplazar valores" o utiliza la opción "Reemplazar valores" en la cinta de opciones bajo la 
pestaña "Transformar". Luego, introduce el valor que deseas reemplazar y el nuevo valor.

Aplicar y cerrar: Una vez completado, haz clic en "Cerrar y aplicar" para guardar los cambios y regresar a la vista principal de Power BI.

#### 5.	Validación de los Cambios:

Una vez que se hayan realizado los cambios en la base de datos, verifica la integridad de los datos y asegúrate de que se hayan agregado correctamente los nuevos campos y se 
hayan aplicado los procedimientos de limpieza de datos.

Realiza pruebas exhaustivas para confirmar que los datos actualizados sean precisos y estén listos para su análisis.

#### 6.	Actualización del Dashboard:

Si es necesario, actualiza las conexiones de datos para reflejar los cambios en la estructura del arvhivo.

Modifica los paneles y visualizaciones existentes según sea necesario para incluir los nuevos datos y campos.

Verifica que el dashboard se actualice correctamente y que todas las visualizaciones muestren la información actualizada de manera precisa.

#### 7.	Documentación:

Documenta todos los cambios realizados en la base de datos y en el dashboard, incluyendo detalles sobre los nuevos campos, procedimientos de limpieza de datos y cualquier 
otra modificación realizada.

Proporciona instrucciones claras y detalladas para replicar los pasos de actualización y modelado en el futuro.

#### 8.	Pruebas y Aprobación:

Realiza pruebas exhaustivas del dashboard actualizado para asegurarte de que funcione correctamente y que los datos se muestren de manera precisa.

Obtén la aprobación de los interesados antes de implementar los cambios en un entorno de producción.






