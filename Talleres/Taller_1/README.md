# Taller 1
## Problema 1
Elija un vocabulario técnico correspondiente a un dominio específico, por ejemplo, nombres científicos de animales. Programe una función tipo autocorrector que dada una palabra cualquiera encuentre la palabra más similar dentro del vocabulario elegido.

Solucion:
La solución proporcionada utiliza una técnica de búsqueda de vecinos más cercanos (KNN) en un espacio vectorial TF-IDF (Term Frequency-Inverse Document Frequency) para encontrar la palabra más similar dentro de un vocabulario técnico específico. Se entreno la KNN con  los 2 vecinos más cercanos. La elección de la métrica "cosine" (coseno) en KNN se debe a que es una medida comúnmente utilizada para calcular la similitud entre vectores en espacios vectoriales. En el contexto de procesamiento de texto, el uso de la similitud del coseno es eficaz para medir la similitud entre las palabras representadas como vectores TF-IDF. 

- Ejemplo Palabras Autocompletadas:\\

Especie: salmon \\
Quisiste decir: salmo-salar o monodon-monoceros?

## Problema 2
A partir del algoritmo de k-vecinos más cercanos cree un modelo que clasifique fotografías según el género de la persona retratada. Justifique por qué
la distancia que usted usó es apropiada para este problema

En este problema tenemos vectores que representan una imagen. Entre más parecidos sean dos vectores (V, W), más parecidas son dos imagenes (y entre más parecido sea un pixel V<sub>ij</sub> de W<sub>ij</sub>, más parecidos son los pixeles).  Por lo tanto, entre menor sea la distancia de un vector a otro, más parecidas son las imagenes.  

Entonces tenemos que usar una distancia que entre más diferente sea un pixel de otro, retorne una distancia más grande, y entre menos diferente sea un pixel de otro, retorne una distancia más pequeña, como lo hace la distancia euclidiana.  
![Matriz de confusion](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_2/image.png?raw=true)

## Problema 3
### a.
Grafique en el plano $\mathbb{R}^2$ la bola de radio r y centro en el origen respecto a la distancia de Minkowski de orden p, donde los parámetros r y p varían entre desde 0.1 a 2 y desde 1 a ∞.

Link a la solucion en Desmos:

[![Ejemplo_Solucion_L1](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_3/image.png?raw=true)](https://www.desmos.com/calculator/htvsj2y3t7)


### b.
Programe un algoritmo que dado n y p genere de forma aleatoria un vector de Rn cuya distancia de Minkowski de orden p al origen sea menor a 0.1.

![Puntos Generados en la bola](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_3/puntos_en_bola.png?raw=true)

![Puntos dentro de la bola](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_3/puntos_dentro_bola.png?raw=true)


## Problema 4
Tómese una foto tip o do cumento y transformela a escala de grises y resolución 400 ×600. Defina una sucesión de imágenes que sea convergente a su foto. Muestre al menos 10 términos de la sucesión incluyendo el elemento 100-ésimo. Como la sucesión es convergente, obtenga el término tal que todos las imágenes siguientes en tienen una distancia (en norma de Frobenius) menor a 0.5 de su foto.

Foto inicial con la que se empezo 

![Foto inicial](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_4/foto_inicial.png?raw=true)

![Foto reconstruida](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_3/foto_final.png?raw=true)

## Problema 5
Demuestre que las normas matriciales inducidas p or las normas vectoriales 1 y ∞, corresp onden a tomar el máximo de la suma de valores absolutos entre
filas y columnas, respectivamente

## Problema 6
### a
Programe un algoritmo que dada una matriz aproxime su norma inducida por la norma vectorial de orden p.

### b 
Usando el algoritmo del ítem anterior estime la norma inducida de ordenes 1, 2, 3 y ∞ para la matríz de Hilbert de tamaño 10 × 10, definida por $H_{10} = [h_{ij}] = \frac{1}{i+j}$.