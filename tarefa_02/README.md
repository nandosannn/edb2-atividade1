# Tarefa 02

## :question: Problema:

Calcule as quantidades de instruções, bem como a
complexidade de pior caso $(O)$ do trecho:

        int numero;
        scanf("%d", &numero);
        
        if(numero % 2 == 0)
                numero = numero + 1;
        else
                numero = numero - 1;
        
        printf("%d", numero);

<br>

## :exclamation: Resposta 

##### Quantidade de intruções:

O trecho do código anterior possui *5 instruções* ao total.

##### Complexidade:

Código | Complexidade
:----- | :----------:
`int numero;`| $O(1)$
`scanf("%d", &numero);`| $O(1)$
`if(numero % 2 == 0);`| $O(1)$
`numero = numero + 1; ou numero = numero - 1;`| $O(1)$
`printf("%d", numero);`| $O(1)$

Portanto, temos:

$T(n) = 1 + 1 + 1 + 1 + 1$

$= 5$

$= O(1)$




