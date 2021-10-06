# Grafos

Grafos são vertices (pontos) e arestas, interligados / relacionados

> **arestas** representam açoes
>
> **vertices / nós** representam entidades
>
> ( redes, ligações, conexões, relações )

---
## Grafos orientados / digrafo


+ Não impoe relação entre os vertices

> ### Exemplo
>
> p.(3,1) !== p.(1,3) 
>
>
>  __wikipedia__
> 
>   + vertices paginas, arestas links
>

---

### Um grafo pode ter :
+ __Lacetes / Loops__: Arestas de um vertice para ele mesmo
+ __Arestas multiplas__: Arestas repetidas 

Os comportamentos acima não ocorrem em __grafos simples__ / __digrafos simples__.

> ### __Question__
> Quantas arestas pode ter um grafo simples de __n__ vertices?
> 
> __R:__ n(n - 1)/ 2 

### __Exemplos matematicos de grafos__
+ K_n -> grafo completo em __n__ vertices 
    + é o grafo simples com n vertices e todas as ( n_2 ) arestas
    + todas os vertices se ligam
+ C_n -> grafo ciclico  de __n__ vertices
    + grafo com n vertices ligados em ciclos

### __Armazenamento classico de grafos__

+ Lista de arestas (___maneira mais simples___) 

    + uma tabela com duas colunas, sendo cada linha uma ligação com um par de vertices (__mesmo para digrafo__) 
        + [1,3]

+ Lista de adjacências

    + uma lista com __n__ linhas. Tendo na linha __i__, os vertices adjacentes   ao vertice __i__ .
    ___adjacentes___: dois vertices são adjacentes se os mesmos formarem uma aresta, isto é: __[ i , j ]__ i e j são adjacentes

+ Matriz de adjacências (___maneira mais matematica___)
    + Tabela __n__ x __n__ onde a entrada ( i *linha*, j *coluna* ) é 1 se [i, j] for uma aresta e 0 se não.
    ___isto é___ uma matriz composta com 0 e 1, indexada pelo numero de vertices.   
                
    ___ex.:___ 1[1  0  1  1 ]

> ### __Nota__
>   Ao ocorrer duas arestas entre os mesmos vertices colocamos o numeral 2. Considerando as regras a baixo.
>
> + Se __G__ for um grafo colacamos __2__ na posição (i,i)
> + Se __G__ for um digrafo colacamos __1__ na posição (i,i)
 
---
**extraknowledge**

_Gephi_ - software de analise de dados