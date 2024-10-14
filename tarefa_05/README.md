# Tarefa 05

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int max = 10;
        int i = 0;
        while(i < max)
                printf("%d", i++);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Complexidade
:----- | :----------:
`int max = 10;`| *1 instrução*
`int i = 0;`| *1 instrução*
`while(i < max)`| *$1 + n$ instruções*
`printf("%d", i++);`| *2n instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+n+2n$

$= 3 + 3n$

Como $n=10$, temos:

$x = 3 + 3.10$

$ = 33$

Portanto, são *$33$ instruções* ao total.
##### Complexidade:

Código | Complexidade
:----- | :----------:
`int max = 10;`| $O(1)$
`int i = 0;`| $O(1)$
`while(i < max)`| $O(n)$ + $O(1)$
`printf("%d", i++);`| $O(n) + O(n)$


Portanto, temos:


$ T(n) = 1 + 1 + 1 + n + 2n$

$ = 3 + 3n$ 

$ = O(n) $

Onde $n = 10$.




