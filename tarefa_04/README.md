# Tarefa 04

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int max = 10;
        int i = 0;
        while(i < max)
                i++;

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Complexidade
:----- | :----------:
`int max = 10;`| *1 instrução*
`int i = 0;`| *1 instrução*
`while(i < max)`| $1 + n$ *instruções*
`i++;`| *n instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+n+n$

$= 3 + 2n$

Como $n=10$, temos:

$x = 3 + 2.10$

$= 23$

Portanto, são $23$ *instruções* ao total.
##### Complexidade:

Código | Complexidade
:----- | :----------:
`int max = 10;`| $O(1)$
`int i = 0;`| $O(1)$
`while(i < max)`| $O(n)$ + $O(1)$
`i++;`| $O(n)$


Portanto, temos:


$T(n) = 1 + 1 + 1 + n + n$

$= 3 + 2n$ 

$= O(n) $

Onde $n = 10$.




