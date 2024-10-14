# Tarefa 01

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int max = 0;
        for(int i = 0; i < max; i++)
                printf("%d", i);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Complexidade
:----- | :----------:
`int max = 0;`| *1 instrução*
`int i = 0;`| *1 instrução*
`i < max;`| *1 instrução*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1$

$=3$

Portanto, são *$3$ instruções* ao total.
##### Complexidade:

Código | Complexidade
:----- | :----------:
`int max = 0;`| $O(1)$
`int i = 0;`| $O(1)$
`i < max;`| $O(1)$

Portanto, temos:

$ T(n) = 1 + 1 + 1$

$ = 3 $

$ = O(1) $




