# Tarefa 08

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int max = 100;
        int a = 0;
        for(int i = 0; i < max; i++){
                a = a + i;
                printf("%d", a);
        }

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int max = 100;`| *1 instrução*
`int a = 0;`| *1 instrução*
`int i = 0;`| *1 instruções*
`i < max;`| *n+1 instruções* 
`i++`| *n instruções*
` a = a + i;`| *n instruções*
`printf("%d", a);`| *n instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+1+n+n+n+n$

$= 4 + 4n$

Como $n = 100$, teremos:

$x = 4 + 4.100$

$=404$

Portanto, são *404 instruções* ao total.


##### Complexidade:

Código | Instruções
:----- | :----------:
`int max = 100;`| $O(1)$
`int a = 0;`| $O(1)$
`int i = 0;`| $O(1)$
`i < max;`| $O(1) + O(n)$ 
`i++`| $O(n)$
` a = a + i;`| $O(n)$
`printf("%d", a);`| $O(n)$

Portanto, temos:

$ T(n) = 1 + 1 + 1 + n + 1 + n + n + n$

$ = 4 + 4n $

$ = O(n) $

Onde $ (n = 10) $.




