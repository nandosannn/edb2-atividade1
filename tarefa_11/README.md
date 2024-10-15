# Tarefa 01

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        for(int i = 0; i < n; i++)
                for(int j = 0; j < n; j++)
                        printf("%d", j);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int i = 0`| *1 instrução*
`i < n;`| $n + 1$ *instruções*
`i++`| *n instruções* 
`int j = 0;`| *n instruções*
`j < n;`| $n(n+1)$ *instruções*
`j++`| $n.n$ *instruções*
`printf("%d", j);`| $n.n$ *instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1 + n +1 + n + n(1 + n + 1 + n + n)$

$= 2 + 4n + 3n²$

Portanto, são *$2 + 4n + 3n²$ instruções* ao total.

##### Complexidade:

Código | Instruções
:----- | :----------:
`int i = 0`| $O(1)$
`i < n;`| $O(n) + O(1)$
`i++`| $O(n)$
`int j = 0;`| $O(n)$
`j < n;`| $O(n²) + O(n)$
`j++`| $O(n²)$
`printf("%d", j);`| $O(n²)$

Portanto, temos:

$T(n) = 1+n+1+n+n+n²+n+n²+n²$

$= 2 + 4n + 3n²$

$= O(n²)$




