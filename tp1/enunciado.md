## Parte 1: Karatsuba!

Dados los siguientes números (completada por su número de padrón)

    a35b411c 
    2d98ef55

con:

    a: dígito del padrón correspondiente a la unidad
    b: dígito del padrón correspondiente a la centena
    c: los dos dígitos del padrón de la izquierda mod 7
    d: dígito del padrón correspondiente a la decena
    e: dígito del padrón correspondiente a la unidad de mil
    f: los dos dígitos del padrón de la derecha mod 9

    Ejemplo. Padrón: 95473

    33544114
    27985155

Se pide:

1. Resuelva la multiplicación paso a paso utilizando el algoritmo de Karatsuba.

2. Cuente la cantidad de sumas y multiplicaciones que realiza y relaciónelo con la complejidad temporal del método.

3. Comparar lo obtenido con el método de multiplicación tradicional. ¿Observa alguna mejora? Analice.

4. ¿Por qué se puede considerar al algoritmo de Karatsuba como de “división y conquista”?

<br/>

## Parte 2: Cuestión de complejidad…

Dado la siguiente relación de recurrencia

    a T(n/b) + O(c)

Con:

    a: 1 + (los dos dígitos del padrón de la izquierda mod 9)
    b: 2 + (los dos dígitos del padrón de la izquierda mod 7)
    c: “n” si su padrón es múltiplo de 4, 
        sino “nlogn” si su padrón es múltiplo de 3,
        sino “n2”  

Se pide:

1. Responda y complete: ¿Qué le falta a la relación de recurrencia para que se pueda aplicar el teorema maestro?

2. Calcular la complejidad temporal utilizando el teorema maestro.

3. Explique paso a paso cómo llega a la misma.
