# Taller 1
## Problema 1
Elija un vocabulario técnico correspondiente a un dominio específico, por ejemplo, nombres científicos de animales. Programe una función tipo autocorrector que dada una palabra cualquiera encuentre la palabra más similar dentro del vocabulario elegido.

Solucion:
La solución proporcionada utiliza una técnica de búsqueda de vecinos más cercanos (KNN) en un espacio vectorial TF-IDF (Term Frequency-Inverse Document Frequency) para encontrar la palabra más similar dentro de un vocabulario técnico específico. Se entreno la KNN con  los 2 vecinos más cercanos. La elección de la métrica "cosine" (coseno) en KNN se debe a que es una medida comúnmente utilizada para calcular la similitud entre vectores en espacios vectoriales. En el contexto de procesamiento de texto, el uso de la similitud del coseno es eficaz para medir la similitud entre las palabras representadas como vectores TF-IDF. 

- Ejemplo Palabras Autocompletadas:
Especie: salmon
Quisiste decir: salmo-salar o monodon-monoceros?

## Problema 2
A partir del algoritmo de k-vecinos más cercanos cree un modelo que clasifique fotografías según el género de la persona retratada. Justifique por qué
la distancia que usted usó es apropiada para este problema

En este problema tenemos vectores que representan una imagen. Entre más parecidos sean dos vectores (V, W), más parecidas son dos imagenes (y entre más parecido sea un pixel V<sub>ij</sub> de W<sub>ij</sub>, más parecidos son los pixeles).  Por lo tanto, entre menor sea la distancia de un vector a otro, más parecidas son las imagenes.  

Entonces tenemos que usar una distancia que entre más diferente sea un pixel de otro, retorne una distancia más grande, y entre menos diferente sea un pixel de otro, retorne una distancia más pequeña, como lo hace la distancia euclidiana.  
![Matriz de confusion](image.png)

## Problema 3
### a.
Grafique en el plano $\mathbb{R}^2$ la bola de radio r y centro en el origen respecto a la distancia de Minkowski de orden p, donde los parámetros r y p varían entre desde 0.1 a 2 y desde 1 a ∞.

Link a la solucion en Desmos:
https://www.desmos.com/calculator/htvsj2y3t7


### b.
Programe un algoritmo que dado n y p genere de forma aleatoria un vector de Rn cuya distancia de Minkowski de orden p al origen sea menor a 0.1.