# Proyecto-Final


![image](https://github.com/bagh1989/Proyecto-Final/assets/172723509/fe3edbf3-c647-4678-b4df-93349e0d2dcd)


**INTRODUCCIÓN**

El procesamiento y análisis de grandes volúmenes de datos es una tarea compleja y multifacética que abarca varias disciplinas esenciales para extraer información valiosa de datos en bruto. En este contexto, el uso de RStudio, una herramienta poderosa y flexible para análisis de datos y programación estadística, resulta fundamental. RStudio proporciona un entorno integrado que facilita el desarrollo de cada uno de los componentes clave en el flujo de trabajo de datos.

La limpieza y transformación de datos constituyen el primer paso crítico en este proceso. A través de RStudio, los datos se preparan para su análisis mediante la eliminación de errores, inconsistencias y duplicados, así como su conversión a un formato adecuado. Este proceso incluye tareas como la normalización de datos, el relleno de valores faltantes y la corrección de errores, asegurando que los datos sean precisos y útiles para el análisis posterior.

El análisis de datos es el siguiente paso, donde se examinan los datos limpios y transformados para descubrir patrones, tendencias y relaciones significativas. Con RStudio, se pueden realizar análisis descriptivos, inferenciales, predictivos y prescriptivos, utilizando una amplia gama de herramientas estadísticas y algoritmos de machine learning. Esta fase es crucial para tomar decisiones informadas y desarrollar estrategias basadas en evidencia.

La visualización de datos, otro componente esencial, implica la representación gráfica de los datos para facilitar su interpretación. RStudio, con su capacidad para generar gráficos y diagramas sofisticados, permite crear visualizaciones efectivas que ayudan a los usuarios a comprender rápidamente las complejidades de los datos. Desde gráficos de barras y líneas hasta dashboards interactivos y mapas geográficos, RStudio ofrece diversas herramientas para comunicar hallazgos de manera clara y concisa.

En el ámbito de la ciencia de datos, RStudio se utiliza para aplicar métodos científicos, procesos, algoritmos y sistemas que extraen conocimiento de los datos. Los científicos de datos pueden desarrollar y validar modelos predictivos, utilizar algoritmos de machine learning y aplicar técnicas de minería de datos para descubrir relaciones ocultas y patrones complejos. La flexibilidad y las capacidades avanzadas de RStudio son esenciales para llevar a cabo estos análisis profundos.

Finalmente, la ingeniería de datos se enfoca en la construcción y optimización de sistemas para recopilar, almacenar y procesar grandes volúmenes de datos. Con RStudio, los ingenieros de datos pueden diseñar y mantener infraestructuras de datos robustas, implementando pipelines de datos y optimizando el rendimiento de los sistemas de procesamiento. Tecnologías como Hadoop y Spark se integran fácilmente con RStudio, proporcionando una base sólida para el flujo continuo de datos.

A.	LIMPIEZA Y TRANSFORMACIÓN DE DATOS:

1.	Limpieza: Primero como descripción general nuestra gestión de datos se basó en la adquisición, organización, almacenamiento y manipulación de la base de datos cuya colección son los datos organizados de manera lógica para obtenerlos los obtuvimos de Kaggle, el archivo inicial descargado es una archivo CVS por lo que los datos se encuentran sin procesar y los extrajimos para ser revisados una vez revisados se cuentan y clasifican para la verificación del conjunto de datos, los datos fueron ordenados en función de varias variables.

2.	Transformación de datos:Para la transformación de los datos utilizamos la función dim para contar el número de observaciones y variables.
Otra de las funciones utilizadas son head y View, donde Head nos muestra las observaciones en el conjunto de datos, mientras que la función View muestra un visor de datos al estilo de una hoja de cálculo donde nos podemos desplazar por filas y columnas.
is.na nos ayuda a la identificación las observaciones con valores faltantes en R etiquetarlos con Verdadero en valores faltantes y Falso sin valores con el fin de inspeccionar la variable Industry en busca de valores faltantes.
Para inspeccionar la observación número 64, nos muestra en el marco de datos.

B.	ANALISIS DE DATOS
La base de datps utilizada esta denominada como “data(proyecto_final)”.
Con esta función podemos verificar la impresión de nuestra tabla para poder revisar los datos que vamos analizar y poder entender que es lo que necesitamos analizar.

<img width="461" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/f590dd1d-3132-4665-b7bd-326bad73178d">

Por medio de este código se puede visualizar toda la información de la base de datos para poder analizar la información que necesitamos desarrollar.

Con la función “STR” se puede visualizar todas las variables que contiene nuestra base de datos que estamos analizando.

<img width="457" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/e64dbf2c-c472-4a8d-abc2-8263576f10c6">

La función “HEAD” muestra las primeras 5 variables que se tienen en la base de datos como se muestra en la siguiente imagen:


<img width="381" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/a8cc52f0-b24d-4b43-adc5-9a02c2f25a07">

La función “TAIL” nos muestra las ultimas variables de la base de datos.

<img width="360" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/d7c1f0af-f453-450e-a6bb-c0dbe205e25b">

La función “summary” nos muestra el resumen de todas variables de nuestra base de datos.

<img width="359" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/a22b508c-160b-4145-91d1-bb9b01829f62">

Lo interesante de la función “attach” es que nos permite ver el resumen especifico de la columna que deseamos revisar lo que nos da una proyección de análisis más limpia. Por ejemplo: con la función “summary() más la columna que deseamos analizar “cliente” nos da el resumen detallado como se muestra en la siguiente imagen:

<img width="441" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/4abb6908-f5b1-4d9f-8d5d-6cfc187d01ae">

Con el comando “summary” sucesivamente se puede ir analizando las columnas que se deseen, para que analice un campo en específico lo cual resulta como beneficio para el análisis que se requiera, podemos usar los siguientes comandos, por ejemplo:

•	mean(wage)

•	mean(age)

•	median(wage)

•	min(age)

•	max(wage)

•	var(wage)

•	sd(wage)

C.	VISUALIZACIÓN DE DATOS
Con la función “hist (columna x, freq = FALSE)” se puede analizar el histograma de los datos en validación para determinar la toma de decisiones de forma efectiva.

<img width="441" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/35472412-de25-45d6-980b-8e4d96ea5395">

La función “hist(log(columna x), freq = FALSE)” permite agrupar la gráfica de la siguiente forma lo cual resulta de beneficio para el análisis en gestión.

<img width="362" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/eeebe49f-4eb9-4cae-a573-ca8d69f2f5d0">

Con la función “lines (density (log (Columna x)), col = 4)” se puede agregar líneas en la gráfica lo que resulta relevante para el análisis de datos, como se muestra a continuación:

•	lines(density(log(columna x)), col = 3)
•	lines(density(log(columna x)), col = 2)

<img width="441" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/3ec1eb05-2de5-4b10-9d16-52138335ad9f">

Variables Categóricas

Para determinar variables categóricas se usa el comando “summary (columna x)” según la columna que se necesita analizar para graficar los campos en análisis.

<img width="441" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/63455af1-f584-4581-a547-aedbcd9a35b8">

D.	CIENCIA DE DATOS

1.	REGRECIÓN LINEAL

<img width="420" alt="image" src="https://github.com/bagh1989/Proyecto-Final/assets/172723509/8a31102d-db1c-403e-b750-1668a696be26">


**Interpretación de los Coeficientes
**
1.	Intercept (Intercepto):
o	Estimate: 1832.89

o	Esto indica el valor esperado de Cliente cuando todas las variables independientes son cero.

o	Significancia: Muy significativa (p < 0.001).

3.	Auto:
o	Estimate: -0.0026

o	El coeficiente sugiere que por cada unidad adicional en Auto, Cliente disminuye en 0.0026 unidades.

o	Significancia: No significativa (p = 0.992).

5.	Ubicación:
o	Estimate: -0.0248

o	El coeficiente sugiere que por cada unidad adicional en Ubicación, Cliente disminuye en 0.0248 unidades.

o	Significancia: No significativa (p = 0.710).

6.	Fecha:
o Estimate: 0.0000001279

o	El coeficiente sugiere que por cada unidad adicional en Fecha, Cliente aumenta en 0.0000001279 unidades.

o	Significancia: No significativa (p = 0.612).

8.	PagoEfectivo:

o	Estimate: -36.1612

o	Si el pago es en efectivo, Cliente disminuye en 36.1612 unidades en comparación con el pago no en efectivo.

o	Significancia: No significativa (p = 0.118).

10.	SeguroSI:

o	Estimate: -0.0564

o	Si el seguro es sí, Cliente disminuye en 0.0564 unidades en comparación con no tener seguro.

o	Significancia: No significativa (p = 0.998).


Estadísticas del Modelo

•	Residual standard error: 1155 (un gran valor indica un modelo que no ajusta bien).

•	Multiple R-squared: 0.0002862 (muy bajo, lo que indica que las variables independientes explican una fracción mínima de la variabilidad en la variable dependiente).

•	Adjusted R-squared: -0.0002143 (ajustado por el número de predictores, aún peor).

•	F-statistic: 0.5718 en 5 y 9986 grados de libertad (df) con un p-valor de 0.7217 (el modelo en conjunto no es significativo).

































