# TM_udemy_reviews

La propuesta es:

0) Analizar el conjunto de muestras que tenemos.
  * 0a) Probar filtrando solo las reviews de más de 5 palabras y ver si las que dejamos afuera son útiles.
  * 0b) Quitar stopwords personalizadas tipo "curso","clase","bien"
  * 0c) Ver cuáles son las palabras que mejor separan las reviews positivas de las negativas.

1) Tomar las reviews, y sacarle el topic del que hablan.
  * 1a) Comparar si las reviews negativas dan más info que si usáramos todo el dataset completo.
  * 1b) Probar filtrando solo las reviews negativas, o probar con todo.
  * 1c) Probar con distinta cantidad de tópicos y ver si podemos separar los clusters.

2) Agrupar las reviews por curso.
  * 2a) Los cursos pueden tener distintas iteraciones (tipo el mismo curso se da todos los años con distinto id). Quizás conviene revisar si el mismo curso tiene distintos id asociados.

3) Distribución de topics x curso
  * 3a) Cuál es el puntaje promedio de cada tópico?
  * 3b) Usar alguna métrica para probar que x cada probabilidad de cada tópico hay un puntaje.
  * 3c) Quizás poner algún tipo de threshold para decir "todo lo que tiene alta probabilidad de tópico 1, asignarle esa etiqueta". La review habla de *ese* topico.
  * 3d) O quizás en vez de poner un threshold y hacer one-hot-encoding, ponderar los tópicos y quedarnos con "esta review tiene X% prob de hablar del topico 1 y Y% prob de hablar del topico 2" - Tipo una review puede hablar de varios tópicos.

4) Asociar las reviews al puntaje final del curso.
  * 4a) Qué tópicos se correlacionan más con el puntaje?
  * 4b) Evaluar cuánto aportan los comentarios sobre cada tópico al puntaje total del curso.
  * 4c) Regresionar el puntaje con los scores de los tópicos.


