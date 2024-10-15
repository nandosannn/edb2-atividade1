# Tarefa 13

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int n = 5;
        int num[n];
        for(int i = 0; i < n; i++)
                if(num[i] % 2 == 0)
                        printf("%d", num[i]);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int n = 5;`| *1 instrução*
`int num[n];`| *1 instrução*
`int i = 0;`| *1 instruções* 
`i < n;`| $n + 1$ *instruções*
`i++`| $n$ *instruções*
`if(num[i] % 2 == 0)`| $n$ *instruções*
`printf("%d", num[i]);`| $n$ *instruções*

Então, $x$ sendo o número total de instruções, temos:

$x = 1 + 1 + 1 + (n+1) + n + n + n$

$= 4 + 4n$

Como $n=5$, temos:

$x=4+4.5$

$=4+20$

$=24$

Portanto, são $24$ instruções* ao total.

##### Complexidade:

Código | Instruções
:----- | :----------:
`int n = 5;`| $O(1)$
`int num[n];`| $O(1)$
`int i = 0;`| $O(1)$ 
`i < n;`| $O(1) + O(n)$ 
`i++`| $O(n)$
`if(num[i] % 2 == 0)`| $O(n)$
`printf("%d", num[i]);`| $O(n)$

Portanto, temos:

$T(n) = 1 + 1 + 1 + (n+1) + n + n + n$

$= 4 + 4n$

$= O(n)$




