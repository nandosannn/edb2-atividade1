# Tarefa 10

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int a = 0;

        for(int i = 1; i < n; i++){
                a++;
                printf("%d", i);
        }

        printf("%d", a);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int a = 0;`| *1 instrução*
`int i = 1;`| *1 instruções*
`i < n;`| *n instruções* 
`i++`| *n instruções*
`a++`| *n instruções*
`printf("%d", i);`| *n instruções*
`printf("%d", a);`| *1 instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+n+n+n+n$

$= 3 + 4n$

Portanto, são *$3 + 4n$ instruções* ao total.


##### Complexidade:

Código | Instruções
:----- | :----------:
`int a = 0;`| $O(1)$
`int i = 0;`| $O(1)$
`i < n;`| $O(n)$ 
`i++`| $O(n)$
`a++`| $O(n)$
`printf("%d", i);`| $O(n)$
`printf("%d", a);`| $O(1)$

Assim, temos:

$ T(n) = 1 + 1 + n + 1 + n + n + n$

$ = 3 + 4n $

$ = O(n) $




