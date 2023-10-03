# Taller 1

## Problema 1
**Descripción:** Elija un vocabulario técnico correspondiente a un dominio específico, por ejemplo, nombres científicos de animales. Programe una función tipo autocorrector que dada una palabra cualquiera encuentre la palabra más similar dentro del vocabulario elegido.

**Solución:** La solución utiliza un enfoque de búsqueda de vecinos más cercanos (KNN) en un espacio vectorial TF-IDF (Term Frequency-Inverse Document Frequency) para encontrar la palabra más similar dentro de un vocabulario técnico específico. Se utiliza KNN con 2 vecinos más cercanos y la métrica "cosine" (coseno) para medir la similitud entre palabras representadas como vectores TF-IDF.

**Ejemplo de Palabras Autocompletadas:**
- Especie: salmon
- ¿Quisiste decir?: salmo-salar o monodon-monoceros?

## Problema 2
**Descripción:** A partir del algoritmo de k-vecinos más cercanos, cree un modelo que clasifique fotografías según el género de la persona retratada. Justifique por qué la distancia que usted usó es apropiada para este problema.

**Justificación:** Se utiliza la distancia euclidiana en este problema ya que las imágenes se representan como vectores y esta distancia mide la similitud entre los vectores de características de las imágenes. Cuanto más parecidos sean los vectores, más parecidas serán las imágenes.

**Resultado:**

- Matriz de Confusión: ![Matriz de Confusión](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_2/image.png?raw=true)

## Problema 3
### a.
**Descripción:** Grafique en el plano \(\mathbb{R}^2\) la bola de radio \(r\) y centro en el origen respecto a la distancia de Minkowski de orden \(p\), donde los parámetros \(r\) y \(p\) varían desde 0.1 hasta 2 y desde 1 hasta ∞.

**Solución:** Se proporciona una solución en Desmos para visualizar la bola de Minkowski en el plano \(\mathbb{R}^2\).

 [Ver Solución en Desmos](https://www.desmos.com/calculator/htvsj2y3t7)

### b.
**Descripción:** Programe un algoritmo que, dado \(n\) y \(p\), genere de forma aleatoria un vector de \(\mathbb{R}^n\) cuya distancia de Minkowski de orden \(p\) al origen sea menor a 0.1.

**Resultado:** 
- Puntos Generados en la Bola: 

![Puntos Generados en la Bola](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_3/puntos_en_bola.png?raw=true)
- Puntos dentro de la Bola: 

![Puntos dentro de la Bola](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_3/puntos_dentro_bola.png?raw=true)

## Problema 4
**Descripción:** Tómese una foto típica o documento y transfórmela a escala de grises y resolución 400 × 600. Defina una sucesión de imágenes que sea convergente a su foto. Muestre al menos 10 términos de la sucesión, incluyendo el elemento 100-ésimo. Como la sucesión es convergente, obtenga el término tal que todas las imágenes siguientes tengan una distancia (en norma de Frobenius) menor a 0.5 de su foto.

**Resultado:** Se muestra la foto inicial y la foto reconstruida con un enfoque iterativo.

- Foto Inicial: 

![Foto Inicial](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_4/foto_inicial.png?raw=true)
- Foto Reconstruida: 

![Foto Reconstruida](https://github.com/coberndorm/Algebra-In-Data-Science/blob/main/Talleres/Taller_1/Punto_4/foto_final.png?raw=true)

## Problema 5
**Descripción:** Demuestre que las normas matriciales inducidas por las normas vectoriales 1 y ∞ corresponden a tomar el máximo de la suma de valores absolutos entre filas y columnas, respectivamente.

## Problema 6
### a.
**Descripción:** Programe un algoritmo que, dada una matriz, aproxime su norma inducida por la norma vectorial de orden \(p\).

### b.
**Descripción:** Usando el algoritmo del ítem anterior, estime la norma inducida de órdenes 1, 2, 3 e ∞ para la matriz de Hilbert de tamaño 10 × 10, definida por \(H_{10} = [h_{ij}] = \frac{1}{i+j}\).
