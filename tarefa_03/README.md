# Tarefa 03

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int max = 0;
        int i = 0;
        while(i < max)
                i++;

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

O trecho do código anterior possui *3 instruções* ao total.

##### Complexidade:

Código | Complexidade
:----- | :----------:
`int max = 0;`| $O(1)$
`int i = 0;`| $O(1)$
`while(i < max);`| $O(1)$

Portanto, temos:

$ T(n) = 1+1+1$

$= 3$

$= O(1) $




