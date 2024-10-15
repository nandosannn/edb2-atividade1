# Tarefa 01

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

       int busca_binaria(int c, int n, int v[])

        int i = 0;
        int f = n - 1;
        while(i <= f){
                int m = i + (f - i) / 2;
                
                if(v[m] == c) {
                        return m;
                
                if(v[m] < c)
                        i = m + 1;
                else
                        f = m - 1;
                }       
                return -1;
                }
        
        
<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

Código | Instruções
:----- | :----------:
`int i = 0;`| *1 instrução*
`int f = n - 1;`| *1 instrução*
`while(i <= f)`| $\log_2 n + 1$ *instruções*
`int m = i + (f - i) / 2;`| $\log_2 n$ *instruções*
`if(v[m] == c)`| $\log_2 n$ *instruções*
`if(v[m] < c)`| $\log_2 n$ *instruções*
`i = m + 1; ou f = m - 1;`| $\log_2 n$ *instruções*
`return -1;`| *1 instrução*

Então, $x$ sendo o número total de instruções, temos:

$x = 1+1+1+\log_2 + \log_2 + \log_2 + \log_2 + \log_2 + 1$

$= 4 + 5.\log_2$

Portanto, são $4 + 5.\log_2$ *instruções* ao total.


##### Complexidade:

Código | Instruções
:----- | :----------:
`int i = 0;`| $O(1)$
`int f = n - 1;`| $O(1)$
`while(i <= f)`| $O(\log_2n) + O(1)$
`int m = i + (f - i) / 2;`| $O(\log_2n)$
`if(v[m] == c)`| $O(\log_2n)$
`if(v[m] < c)`| $O(\log_2n)$
`i = m + 1; ou f = m - 1;`| $O(\log_2n)$
`return -1;`| $O(1)$

Portanto, temos:

$T(n) = 1 + 1 + \log_2n + 1 + \log_2n + \log_2n + \log_2n + \log_2n + 1$

$= 4 + 5\log_2n$

$= O(\log_2n)$




