# <img style="float: left; padding-right: 0.2cm; width: 9.0cm" src="https://th.bing.com/th/id/R.69cb7735a422db336e0d49d0dc89c21c?rik=YmUVpMyvcM4B%2bw&pid=ImgRaw&r=0">

## Análisis de rendimiento del Campeonato Nacional de Futbol Chileno Profesional entre los años 2010 a 2020

Este proyecto surgió por el fanatismo que tenemos hacia el futbol, los torneos nacionales y cada amistoso que se ha desarrollado que hemos puesto nuestra atencion, desarrollando un gran sentimiento de amor y aprecio por el deporte, generando lazos con equipos determinados por su juego, cordinacion y determinacion por ganar.
Dando un paso mas alla, nos intrigo el funcionamiento de cada equipo para que nos den el espectaculo que tanto nos gusta ver en vivo, y nos concentramos en analizar estadisticas de los campeonatos nacionales de fútbol profesional chileno de primera división.

Utilizamos como fuentes de información las paginas siguientes:

-Wkipedia, que nos facilitaba la obtención de resultados positivos, ya que poseia varias tablas con información útil respecto al año de torneo que se requería, y era mas sencillo aplicar web scraping.

-Tansfermarkt, el cual provee información sobre valores de mercados de los equipos, vlores de mercado de los jugadores, ingresos obtenidos por venta de jugadores de los equipos por año, costos obtenidos por la compra de jugadores de los equipos por año, etc.

Nuestra propuesta fue analizar las estadisticas de torneos y mundiales futbolisticos de la ultima decada; donde tocamos temas como:

-Estadisticas descriptivas de desempeño por equipo en cada año que participaron del torneo

-Comprender la distribucion por region de los equipos en permanencia en primera division

-Relacion entre popularidad (en base a hinchada) y rendimiento de un equipo por torneo 

-Relacion del balance total por equipo en concepto de venta y compra de jugadores y su rendimiento

1-¿Existe correlación entre la popularidad de un equipo y su rendimiento en los torneos?

2-¿Cómo es la distribución de los equipos por región participantes de los torneos por año?

3-¿Existe correlación entre ser un equipo de región y el rendimiento de dicho equipo?

4-¿De qué regiones son los equipos con mejor rendimiento?

5-¿Existe correlación entre el balance total en concepto de compra y venta de jugadores de los 3 mejores equipos y los 3 peores 
equipos de los torneos por años y su rendimiento en los torneos?

6-¿Serán los equipos que más invierten los con mejor rendimiento?

## Observaciones y hallazgos

Los resultados hallados durante el estudio de lo planteado los responderemos en base a la relacion que tienen con respecto a las preguntas de investigación planteadas:

1) Respondiendo a la pregunta 1, utilizamos el dataset de los equipos que permanecieron en primera división durante todo el intervalo de tiempo medido para el proyecto. Es importante resaltar que el numero de datos ingresados son bajos ya que el Nº de equipos que se mantuvo en primera división durante los 10 años en que se midio el proyecto fueron 9. De esta manera las metricas utilizadas como el MSE y R2, dificilmente son posibles de analizar correctamente debido a la baja cantidad de datos. Por lo tanto el análisis para este apartado estaría sesgado debido a la baja cantidad de datos.

2) Para la pregunta dos apreciamos que gran parte de los equipos que han estado en primera división estos 10 útlimos años pertenecen a la región metropolitana. Se puede apreciar que en general estos equipos son los que presentan un mayor gasto en compra y venta de jugadores, lo que habla del poder adquisitivo de estos equipos en comparación con los equipos de regiones. También es notoria la diferencia en la capacidad de los estadios, superando hasta en casi 4 veces el tamaño de los estadios de los equipos de regiones pequeños. 

3) Para las preguntas 3 y 4, al analizar el dataframe de rendimiento acumulado, vemos que 6 de los 7 equipos de la región metropolitana se han mantenido sin descender a lo largo del intervalo de tiempo estudiado. Esto puede ser indicativo de que al ser un equipo de región se tiene mayores probabilidades de descender a la segunda división del fútbol chileno. No consideramos el ser de región como variable categórica en el análisis ya que pudimos llegar a esta conclusión mediante el dataframe de rendimiento acumulado.

4) Y con respecto a las ultimas dos preguntas, en base al modelo multilineal con regularización seleccionado(regresión Lasso con alfa igual a 1), notamos que las variables ingresos y costos no tienen un peso significativo en la predicción de cantidad de puntos obtenidos por equipo, por lo tanto estas variables no estan influyendo en los rendimientos de los equipos.

Para simplificar un poco los datos hemos analizado cual a sido el top 5 de los equipos que sobresalieron (y que han ganado) en los torneos de cada año.

De este analisis se han destacado tres: La Universidad de Chile, la Universidad Catolica y el Colo-Colo
# <img style="float: center; padding-right: 0.5cm; width: 9.0cm" src="https://th.bing.com/th/id/R.eb9f4b9c1f6a937ae39c3eb85241bb28?rik=V3F7vqqe4izTOQ&pid=ImgRaw&r=0&sres=1&sresct=1">

1.) De la Universidad de Chile vemos que ha quedado en el top 5 ocho veces (con escepción en los años 2013, 2015 y 2019) y ha ganado el torneo de los años 2011 y 2012

2.) Le sigue la Universidad Catolica que ha logrado estar 9 veces dentro de los 5 mejores (donde no pudieron en los años 2014 y 2017), y la sorpresa es que han ganado 7 de 11 torneos en los ultimos 10 años analizados, con una racha de tres torneos ganados entre los años 2018 a 2020. Se convierte en el máximo triunfador de la decada.

3.) Por ultimo tenemos a Colo-Colo, que comparado con el resto ha permanecido en el top 5 10 veces, con la unica escepcion el año 2020 donde tuvieron muchas complicaciones. Y solo han ganado dos torneos, el de 2014 y 2017

Una comparacion interesante es que colo-colo ha ganado en los mismos años en que la UC no a podido quedar entre los 5 mejores, lo que podria indicar que habria una relacion entre el desempeño de ambos equipos, donde si a uno le esta yendo mal, el otro aprovecha para ganar confianza y mejorar en sus partidos 
