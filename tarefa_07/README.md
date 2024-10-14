# Tarefa 07

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int max = 10;
        for(int i = 0; i < max; i++)
                printf("%d", i);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int max = 10;`| *1 instrução*
`int i = 0`| *1 instrução*
`i < max`| *n + 1 instruções*
`i++`| *n instruções* 
`printf("%d", i);`| *n instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+n+n+n$

$= 3 + 3n$

Como $n = 10$, teremos:

$x = 3 + 3.10$

$=33$

Portanto, são *33 instruções* ao total


##### Complexidade:

Código | Complexidade
:----- | :----------:
`int max = 10;`| $O(1)$
`for(int i = 0; i < max; i++)`| $O(1) + O(n)+O(1) + O(n)$
`printf("%d", i);`| $O(n)$

Portanto, temos:

$ T(n) = 1 + 1 + n + 1 + n + n$

$ = 3 + 3n $

$ = O(n) $

Onde $ (n = 10) $.




