# Análisis Costo-Beneficio  📊

**Descripción del Proyecto**

En este proyecto se trabaja sobre una base de datos con 8847 filas/transacciones (sin duplicados) y 10 variables iniciales. Tras una limpieza de datos y normalización de los mismos para asegurar la calidad e integridad de la base de datos, se procede a un análisis en profundidad de la actividad de ventas de una empresa mayorista en un ejericicio económico del 2012 al 2014. 
La finalidad del análisis consiste en identificar los puntos fuertes de la empresa y crear estratégias para potenciarlos, así como identificar oportunidades de crecimiento en áreas o sectores de la emrpesa que estén generando pérdidas o que tengan los márgenes de beneficios estancados.

**Acciones**

- Limpieza y normalización de datos

- EDA exploratorio para entender la estructura inical de la base de datos, identificar qué problemas previos presenta (datos faltantes, duplicados, incoherencia e incosistencia en los datos).

- Análisis de correlaciones a través de estadísticos descriptivos y tablas dinámicas.

- Identificación de valores atípicos.

- Identificación de patrones entre variables.

- Cálculo de nuevas columnas que potencien los resultados de análisis.

- Análisis del coste, beneficio y volúmen de ventas por país, línea de producto, subcategoría de producto y compañía.

- Análisis temporales.

- Cálculo de KPIs.



**Problemas encontrados** 🐧
- El tratamiento de los datos faltantes en la base de datos para la variable "Unit Price". El precio medio de los productos calculados en base al promedio por trimestre fue muy difícil de trasladar a la base de datos con las funciones de Excel.
- Dado el sesgo hacia la derecha y la alta dispersión en Profit, algunos productos son significativamente más rentables que otros. La alta variabilidad sugiere que existen productos o líneas de negocio que contribuyen desproporcionadamente a las ganancias. A partir de esta información, la empresa podría enfocarse en identificar y potenciar estos productos de alto margen, además de evaluar la posibilidad de reducir costos en aquellos de bajo margen o alto costo, para mejorar la rentabilidad en general.
- Impacto del volumen de ventas: La correlación fuerte y positiva entre Quantity y Cogs Total (0.7573) en la tabla de correlación es coherente con el alto rango y variabilidad de Quantity en los estadísticos descriptivos. Esto sugiere que, mientras se venden muchas unidades de ciertos productos, los costos asociados también aumentan significativamente, afectando potencialmente la rentabilidad. Además, la correlación negativa entre Quantity y Profit (-0.4289) indica que un volumen de ventas alto no siempre se traduce en mayor rentabilidad. Esto podría indicar que algunos productos de alto volumen tienen márgenes muy bajos, reduciendo las ganancias globales.
- Se detecta un aumento muy significativo en Proft a partir del último año que no va acompañado de ningún cambio en volúmen de ventas, incorporación de algun nuevo país o nueva empresa de retailer ni tampoco de un márgen de beneficio mayor. No se consgiue detectar ningún cambio en los patrones de ventas que logre explicar este nivel de beneficios mucho más alto que los anteriores ni a su vez una explicación de porque no aumenta significativamente junto con el Profit el Gross Margin.

**Estructura del Proyecto**

  **├──** VentasDataM.xlsx                            [Datos limpios, EDA, análisis y KPIs]
 
  **├──** VentasProductos_Data                        [Datos crudos convertidos a Tabla]
  
  **├──** README.md                                   [Descripción del proyecto]


**Instalación y requisitos**

Para replicar el análisis se requiere de Microsoft Excel 2016.

**Próximos Pasos**
 - Se recomienda obtener más datos que signifiquen nuevas variables, para facilitar el reconocimiento de patrones en los datos que expliquen las causas del aumento de beneficios sin que conlleve un aumento de los márgenes. 

 - Hacer un análisis más exhaustivo de UnitPrice (precio por producto) y UnitCogs (coste del producto) y ver su relación con el aumento de beneficios.

 - Buscar estudios de caso concreto en las intersecciones temporales donde el beneficio sube agresivamente.

**Resultados y Conclusiones** 🕵️‍♀️
-  El crecimiento en los ingresos está alineado con el aumento en la cantidad de productos vendidos, pero la rentabilidad, en términos de margen bruto, puede sacrificarse en algunos casos para generar ingresos. 
- Los productos que más contribuyen a los ingresos no siempre son los que ofrecen mayores márgenes, y la cantidad vendida no garantiza una mejora en la rentabilidad.
- Líneas de productos que generan pérdidas se recomienda retirarse de su venta, como en el caso de "Outdoor Protection"
- Se recomienda hacer una gran campaña de marketing de productos de Golf, ya que a pesar de su bajo volúmen de ventas es la línea de producto que más beneficios nos proporciona.
- Se recomienda hacer un reajuste en los costes de los productos para potenciar las ventas y/o mejorar el márgen de beneficio. 

**Contribuciones**

 Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, por favor abre un pull request o una issue.

**Autor y Agradecimientos**

Gracias a todos los compañeros del Bootcamp de DataAnalytics Hackio y sus profesores por el acompañamiento en el desarrollo de este proyecto que estuvieron guíandome para conseguir las mejores técnicas en el tratamiento de datos faltantes e impulsaron nuevas ideas para los análisis. 🙏🏼

Autora: Marta Blanco Arévalo

Linkedin: https://www.linkedin.com/in/marta-blanco-arev/
