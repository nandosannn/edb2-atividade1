# Tarefa 09

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int n;
        scanf("%d", &n);
        for(int i = 0; i < n; i++){
                printf("%d", i);
        }

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int n;`| *1 instrução*
`scanf("%d", &n);`| *1 instrução*
`int i = 0;`| *1 instruções*
`i < n;`| *n+1 instruções* 
`i++`| *n instruções*
`printf("%d", i);`| *n instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+1+n+n+n$

$= 4 + 3n$

Portanto, são *$4 + 3n$ instruções* ao total.

##### Complexidade:

Código | Instruções
:----- | :----------:
`int n;`| *1 instrução*
`scanf("%d", &n);`| $O(1)$
`int i = 0;`| $O(1)$
`i < n;`| $O(1) + O(n)$ 
`i++`| $O(n)$
`printf("%d", i);`| $O(n)$

Assim, temos:

$ T(n) = 1 + 1 + 1 + n + 1 + n + n$

$ = 4 + 3n $

$ = O(n) $




