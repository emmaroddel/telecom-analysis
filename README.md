# telecom-analysis

El objetivo del proyecto es evaluar el comportamiento de los clientes de una empresa de telecomunicaciones en Latinoamérica, ConnectaTel.
Trabajaremos con información registrada hasta el año 2024, lo cual permitirá analizar el comportamiento del negocio dentro de ese periodo.


##Pasos del proyecto

1 -  **Carga y exploración del Dataset**

Primero necesitamos entender en lo que vamos a trabajar exportando el dataset. con pandas y numpy logramos ver la información que contenía el dataset y validar cuanta información será necesaria limpiar, reacomodar y/o sustituir.

2 - **Identificación de problemas de calidad de datos**

En este paso es importantísimo enfocarnos en validar que los datos que estamos viendo estén correctos, ya qwue se pueden encontrar valores nulos, valores inválidos y/o sentinels que puedan estar estropeando la calidad de nuestro dataset. 
De igual manera tenemos que estandarizar nuestras columnas que contengan fechas para que no se encuentren errores en futuros análisis.

3 - **Limpieza básica de datos**

Un a vez que identificamos los datos nulos, los valores inválidos, los sentinels y las fechas imposibles, procedemos a la limpieza del dataset donde estaremos reemplazando los sentinels con la mediana, o bien, eliminando valores imposibles.

4 - **Resumen estadístico de uso por usuario**

Ya que nuestros datos están limpios, creamos dos columnas que nos den a conocer la cantidad de mensajes y la cantidad de llamadas por separado, para que con esta información podamos ver las cantidades totales, media, minimo, Q1, Q3 y máximo, y con esto tener la información preparada para plasmarla de una manera más entendible.

5 - **Visualización de distribuciones**

Con la información recabada en los pasos anteriores, y utilizando histogramas, creamos tablas que demuestren la distribución de nuestros usuarios dividida por edad, cantidad de mensajes por usuario, cantidad de llamadas por usuario y cantidad de minutos en llamada por usuario. De esta forma podemos ver hacia donde están sesgadas nuestras distribuciones.

6 - **Identificación de Outliers**

Usando boxplot, validamos las mismas gráficas para identificar valores atípicos, outliers. Además de utilizar boxplot, validamos también nuestros outliers utilizando el método IQR el cual nos confirmará cuantos Outliers exactos tenemos en cada una de nuestras distribuciones.

7 - **Visualización de la segmentación de clientes**

Además de validar toda la información de los usuarios, es importante también entender a que público se está llegando con más frecuencia y que tipo de clientes tenemos en cuanto al uso del servicio. Así que, con countplot, haremos unas graficas para confirmar que tipo de clientes estamos teniendo y cuanto es el uso que se tiene por cliente.

8 - **Insight ejecutivo para Stakeholders**

Por ultimo, para el entregable de calidad realizamos una traducción de todos los datos recabados del analisis que responderán preguntas accionables para el negocio, enfocadas en segmentación, patrones de uso y oportunidades comerciales.
