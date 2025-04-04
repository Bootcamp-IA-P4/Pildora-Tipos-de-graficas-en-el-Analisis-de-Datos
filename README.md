# Pildora Tipos de graficas en-el Análisis de Datos

El mundo esta lleno de datos, sin embargo es todo un arte interpretarlos y representarlos, este es el propósito de este repositorio darte unas pinceladas para que saques el artista que hay en ti.


Índice:

- [Recursos útiles](#Recursos-útiles)
- [Tipos de gráficas y cuando usarlas](#Tipos-de-gráficas-y-cuando-usarlas)
- [Herramientas en Python](#Herramientas-en-Python)
- [Errores comunes](#Errores-comunes)
- [Buenas Prácticas](#Buenas-prácticas)

## Recursos útiles

* Tipos de gráficos de datos y cómo crearlos en Python [crear gráficas en python](https://www.datacamp.com/es/tutorial/types-of-data-plots-and-how-to-create-them-in-python)
* Ejemplos de uso de gráficos [tipo graficas](https://uni.edu.gt/noticias/tipos-de-graficas/)
* Guía práctica para machine learning [gráficos data science](https://iddigitalschool.com/bootcamps/tipos-de-graficos-para-data-science-y-data-analytics-guia-practica/)
* el arte de mostrar información:[Edward Tufte](https://www.linkedin.com/pulse/edward-tufte-el-arte-de-mostrar-informaci%C3%B3n-rafael-l%C3%B3pez-callej%C3%B3n/)
*  Gráficar con barras divergentes en python: [graficar con barras python](https://r-charts.com/es/parte-todo/grafico-barras-divergentes-ggplot2/)
*  Cómo elegir el gráfico correcto para visualizar datos abiertos: [guía para visualizar datos](https://datos.gob.es/es/blog/como-elegir-el-grafico-correcto-para-visualizar-datos-abiertos)
* El arte y la ciencia de visualizar datos: [el arte de los datos](https://egobiernoytp.tec.mx/es/blog/el-arte-y-la-ciencia-de-visualizar-datos)
*  [Errores en la visualizacion datos](https://tcagency.es/errores-de-visualizacion-de-datos/)



## ¿Por qué visualizar los datos?
Su objetivo es ayudar a nuestra comprensión de los datos aprovechando el sistema visual humano altamente sintonizado para ver patrones, detectar tendencias e identificar valores atípicos.

Antes de continuar me gustaría presentarte a un personaje clave:
> En 1975, [Edward Tufte](https://es.wikipedia.org/wiki/Edward_Tufte), un joven profesor en Princeton, sentó las bases del visual analytics. Hoy es profesor emérito en Yale y es reconocido como una figura clave en la visualización de datos, siendo considerado el “Leonardo da Vinci de los datos”. Entre 2001 y 2006 escribió cuatro libros fundamentales sobre el tema. Sus ideas destacan la importancia de eliminar elementos decorativos e innecesarios en los gráficos, enfocándose en mostrar solo la información relevante y explicativa.


## Tipos de gráficas y cuando usarlas
Ahora si vamos con el plato fuerte de esta píldora:

### Desviación:
Sirve para subrayar las variaciones numéricas desde un punto de referencia fijo. Habitualmente, el punto de referencia es cero, pero también puede ser un objetivo o un promedio a largo plazo. Además, este tipo de gráficos resultan útiles para mostrar sentimientos (positivo, neutral o negativo).  comparar resultados vs. objetivos. Por ejemplo, ingresos esperados vs. reales, o encuestas con opiniones positivas/negativasLos gráficos más frecuentes son:

#### Barra Divergente
Un gráfico de barras estándar simple que permite manejar valores de magnitud tanto negativos como positivos.

 Usos: Muy útil para comparar resultados vs. objetivos. Por ejemplo, ingresos esperados vs. reales, o encuestas con opiniones positivas/negativas

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(17).png)

#### Tabla de columna
Divide un valor único en 2 componentes contrastables.

Usos: Útil para comparar proporciones binarias, como sexo o elecciones (masculino/femenino).

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(10).png)

### Correlación
Útil para mostrar la relación entre dos o más variables. Conviene tener en cuenta que, a menos que les diga lo contrario, muchos lectores asumirán que las relaciones que les muestra son causales. Estos son algunos de los gráficos.

#### Gráfico de dispersión
La forma estándar de mostrar la relación entre dos variables continuas, cada una de las cuales tiene su propio eje.

Usos: Para estudiar cómo se relacionan dos variables, como ingresos vs. gasto, o edad vs. rendimiento.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(16).png)

#### Línea del tiempo
Una buena manera de mostrar la relación entre una cantidad (columnas) y un ratio (línea).

Usos: Muestra simultáneamente una cantidad absoluta (barras/línea) y un ratio (línea secundaria). Ideal para comparar métricas como ventas absolutas vs. porcentaje de crecimiento.


![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(9).png)

### Clasificación
Es necesario clasificar variables numéricas cuando la posición de un elemento en una lista ordenada es más importante que su valor absoluto o relativo. A través de los gráficos dispuestos a continuación es posible resaltar los puntos de interés.

#### Gráfico de barras
Este tipo de visualizaciones permiten mostar los rangos de valores de forma sencilla cuando se ordenan.

Usos: Ideal para rankings, como ventas por producto o rendimiento por empleado.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(15).png)

#### Diagrama tira de puntos
Los puntos están ordenados en una tira. Esta distribución ahorra espacio para diseñar rangos en múltiples categorías.

Usos:  Alternativa más limpia y compacta a las barras, especialmente útil cuando hay muchas categorías.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(8).png)

### Distribución
Este tipo de gráficos buscan resaltar una serie de valores dentro de un conjunto de datos y representar con qué frecuencia ocurren. Es decir, se utilizan para mostrar cómo se distribuyen las variables a lo largo del tiempo, lo que ayuda a identificar valores atípicos y tendencias.

La forma en sí misma de una distribución puede ser una forma interesante de resaltar la falta de uniformidad o igualdad en los datos. Las visualizaciones más recomendadas para representar, por ejemplo, una distribución por edad o sexo son las siguientes:

##### Histograma
Es la forma más habitual de mostrar una distribución estadística. Para desarrollarlo se recomienda mantener un pequeño espacio entre las columnas para, así, resaltar la "forma" de los datos.

Usos: Se usa para analizar la frecuencia, como distribución de edades, tiempos de respuesta o precios. 

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(14).png)

#### Gráfico de cajas
Eficaz para visualizar distribuciones múltiples mostrando la mediana (centro) y el rango de los datos.

Usos: Resume la mediana, cuartiles y posibles valores atípicos. Muy útil en análisis estadístico.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(7).png)

#### Pirámide poblacional
Conocido por mostrar la distribución de la población por sexo. De hecho, se trata de una combinación de dos gráficos de barras horizontales compartiendo el eje vertical.

Usos: Muestra la distribución de población por grupos de edad y sexo.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(6).png)

### Cambios en el tiempo
A través de esta combinación de variables numéricas es posible dar énfasis a tendencias cambiantes. Estos pueden ser movimientos cortos o series extendidas que atraviesan décadas o siglos. Elegir el período de tiempo correcto a representar es clave para ofrecer un contexto al lector.

#### Línea
Es la forma estándar para mostrar una serie temporal cambiante. Si los datos son muy irregulares puede ser útil emplear marcadores que ayuden a representar puntos de datos.

Usos: Seguimiento de KPIs, como tráfico web por mes o crecimiento de usuarios

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(13).png)

#### Mapa de calor calendario
Sirve para mostrar patrones temporales (diario, semanal, mensual). Es necesario ser muy precisos con la cantidad de datos.

Usos: Ideal para visualizar patrones temporales como actividad diaria, asistencia, o ventas a lo largo del año.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(5).png)

### Magnitud
Útil para visibilizar comparaciones de tamaño. Estas pueden ser relativas (simplemente pudiendo ver más grande/mayor) o absolutas (requiere ver diferencias más específicas). Por lo general, muestran variables que pueden ser contadas (por ejemplo, barriles, dólares o personas), en lugar de una tasa calculada o un porcentaje.

#### Columnas
Una de las maneras más comunes de comparar el tamaño de las cosas. El eje siempre debe comenzar en 0.

Usos: Comparar cantidades totales, como presupuesto por departamento o población por ciudad.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(12).png)

#### Gráfico de Marimekko
deal para mostrar el tamaño y la proporción de los datos al mismo tiempo, y siempre y cuando, los datos no sean muy complejos.

Usos: Excelente para visualizar composición de mercados.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(4).png)

### Parte de un todo
Este tipo de combinaciones numéricas son útiles para mostrar cómo una entidad en sí misma puede dividirse en los elementos que lo conforman. Por ejemplo, es común utilizar la parte de un todo para representar la asignación de unos presupuestos o resultados electorales.


#### Gráfico de tarta
Uno de los gráficos más comunes para mostrar datos parciales o completos. Conviene tener presente que no es fácil comparar de forma precisa el tamaño de los distintos segmentos.

Usos: Muy usado en reportes para mostrar distribución de presupuestos, participación de mercado

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(11).png)

#### Diagrama de Venn
Limitado a representaciones esquemáticas que permiten mostrar interrelaciones o coincidencias.

Usos: Representa conjuntos y sus intersecciones. Por ejemplo: usuarios que usan App A, App B, o ambas.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(3).png)

### Espacial
Se recurre a este tipo de gráficos cuando las ubicaciones precisas o los patrones geográficos en los datos son más importantes para el lector que cualquier otra cosa. Algunos de los más utilizados son:

#### Mapa coroplético
Se trata del enfoque estándar para colocar datos en un mapa.

Usos: Normalmente se aplica sobre un mapa real para mostrar intensidad por región (como casos por estado, ingresos por país).

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(2).png)

#### Mapa de flujo
Es utilizado para mostrar un movimiento de cualquier tipo dentro de un mismo mapa. Por ejemplo, puede emplearse para representar movimientos migratorios.

Usos: Muestra movimiento o migración de un lugar a otro, muy útil en logística o migraciones humanas.

![](https://github.com/Bootcamp-IA-P4/Pildora-Tipos-de-graficas-en-el-Analisis-de-Datos/blob/main/img/image%20(1).png)

## Herramientas en Python 

**Librerías Clave:**

*   Matplotlib: La base y el motor de graficación. Ofrece control total sobre cada elemento del gráfico.
*   Seaborn: Construida sobre Matplotlib, simplifica la creación de gráficos estadísticos atractivos y fáciles de usar.
*   Plotly: Librería moderna para gráficos interactivos, ideales para dashboards y exploración dinámica.

## 🎨 Matplotlib: La Base Fundamental
### 🤔 ¿Qué es y Por Qué?

Matplotlib es la librería base para graficar en Python, inspirada en MATLAB. Se creó para dotar a Python de capacidades robustas de graficación 2D (y algo de 3D). Es la base de muchas otras librerías.

### ✨ Características Clave:

*   **Control Total:** Permite personalizar casi cada elemento de un gráfico (líneas, colores, etiquetas, etc.).
*   **Flexibilidad:** Puedes crear una enorme variedad de gráficos estáticos.
*   **Interfaz Dual:** Ofrece una interfaz rápida (pyplot) y una más estructurada y potente Orientada a Objetos (OO).

## 📈 Seaborn: Belleza Estadística Fácil

### 🤔 ¿Qué es y Por Qué?

Seaborn está construida sobre Matplotlib para simplificar la creación de gráficos estadísticos atractivos. Busca facilitar la visualización de relaciones y distribuciones con menos código y mejor estética por defecto. Excelente integración con Pandas.

### ✨ Características Clave:

*   **Alto Nivel:** Funciones directas para gráficos estadísticos comunes (boxplots, violinplots, heatmaps, pairplots).
*   **Integración con Pandas:** Funciona perfectamente pasando DataFrames y nombres de columnas.
*   **Estética Mejorada:** Estilos y paletas de colores por defecto más cuidados.
*   **Enfoque Estadístico:** Muchas funciones calculan e integran agregaciones (medias, IC).

## ✨ Plotly: Interactividad al Poder

### 🤔 ¿Qué es y Por Qué?

Plotly es una librería moderna para crear gráficos interactivos (zoom, pan, hover) basados en HTML/JavaScript. Nace para cubrir la necesidad de visualizaciones dinámicas para web, dashboards (Dash) y exploración detallada.

### ✨ Características Clave:

*   **Interactividad:** Su gran ventaja. Permite explorar los datos directamente en el gráfico.
*   **Web Friendly:** Ideal para embeber en webs, notebooks, Dash.
*   **Plotly Express (px):** Interfaz de muy alto nivel (similar a Seaborn) para crear gráficos complejos rápidamente.
*   **Estética Moderna:** Gráficos pulidos y profesionales.
*   **Offline/Online:** Funciona localmente o integrado con Plotly Chart Studio.


## Errores comunes

Independientemente de la herramienta que uses, ten en cuenta estos errores:

*    **No Limpiar Datos Primero:** Intentar visualizar datos sucios (valores faltantes, tipos incorrectos, outliers) lleva a resultados erróneos.
*    **Elegir el Gráfico Incorrecto:** Usar un gráfico que no se adapta a los datos o la pregunta que intentas responder.
*    **Sobrecargar el Gráfico (Chart Junk):** Añadir elementos visuales innecesarios que distraen o confunden.
*    **Falta de Contexto:** Omitir etiquetas claras en los ejes (con unidades), un título descriptivo o una leyenda.
*    **Escalas Engañosas:** Manipular las escalas de los ejes para exagerar o minimizar diferencias.
*    **Uso Inadecuado del Color:** Usar demasiados colores, paletas no intuitivas o no accesibles.
*    **Confundir Correlación con Causalidad:** Asumir que una relación entre dos variables implica que una causa la otra.

## Buenas Prácticas 

Sigue estas buenas prácticas para crear visualizaciones efectivas:

*   **Define el Propósito:** ¿Qué quieres comunicar con el gráfico?
*   **Conoce tu Audiencia:** ¿Quién verá este gráfico y qué conocimientos tienen?
*   **Prepara tus Datos:** Limpia, transforma y estructura tus datos antes de graficar.
*   **Elige el Gráfico Adecuado:** Selecciona el tipo de gráfico que mejor se adapte a tus datos y objetivos.
*   **Simplifica tu Diseño:** Elimina elementos visuales innecesarios y enfócate en los datos.
*   **Etiqueta Claramente:** Asegúrate de que tu gráfico sea fácil de entender proporcionando etiquetas y contexto.
*   **Usa el Color con Intención:** Elige colores que destaquen la información importante y sean accesibles.
*   **Sé Honesto con las Escalas:** Evita manipular las escalas de los ejes para distorsionar los datos.
*   **Pide Feedback:** Muestra tus gráficos a otros y pide su opinión para mejorar la claridad y la efectividad.
