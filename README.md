# primeiro trabalho de eda

## @andre-filho e @jppgomes

## O que faz e como executar na minha máquina?
O arquivo utilizado da atividade é o trabalho1.cpp.

Caso não tenha, instale o g++:
```bash
    $ apt install g++
```

Para rodá-lo use:

```bash
    $ g++ trabalho1.cpp && ./a.out
```

Então, dentro da aplicação você deverá inserir um número entre 1 e 10.000, como pedido pela interface. O próximo passo é uma confirmação quanto a execução do _case_ de 100k elementos, fica o aviso: **a geração da árvore avl de 100k elementos toma um pouco de tempo**.

A aplicação então realizará as operações de busca em vetores e árvores com tamanhos variados e mostrará o tempo que cada um precisou para rodar a busca, comparando o desempenho dos algoritmos.

**Obs.:** para que os algoritmos rodem em condições iguais, os vetores são gerados com númerais em linha (1..100, 1..1000, 1..10000, etc). O retorno de cada pesquisa segue o seguinte padrão: 

```bash
    <resposta> <nome> (<tamanho_pesquisa>) time: <tempo_execucao>
```

A resposta é **-1 para não encontrado** e o **índice do vetor se encontrado**. Para a **árvore AVL o retorno será o valor**.

Além disso, o tempo de execução (em segundos), tem precisão de 3 casas decimais. Assim sendo, caso o tempo de execução for menor que 0.000 será impresso como 0.

Exemplo de execução da aplicação:
```bash
    Digite um número entre 1 e 100.000 para começar a aplicação
    99999
    deseja rodar o caso de 100k itens? [s/n]
    s
    gerando vetores
    gerado vetor de 100 itens
    gerado vetor de 1000 itens
    gerado vetor de 10000 itens
    gerado vetor de 100000 itens
    vetores gerados
    gerando arvores
    gerada arvore de 100 nos
    gerada arvore de 1000 nos
    gerada arvore de 10000 nos
    a geração da arvore de 100.000 nós demora um pouco. Aguarde...
    gerada arvore de 100000 nos
    arvores geradas!
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    executando com 100 dados
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    -1 avl (100 nodes) time: 0.001
    -1 sentinel (100 units) time: 0
    -1 sequential (100 items) time: 0
    -1 binary (100 items) time: 0
    -1 tabular (100 items) time: 0.001
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    executando com 1000 dados
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    -1 avl (1k items) time: 0.001
    -1 sentinel (1k items) time: 0.002
    -1 sequential (1k items) time: 0.003
    -1 binary (1k items) time: 0
    -1 tabular (1k items) time: 0
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    executando com 10000 dados
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    -1 avl (10k items) time: 0.002
    -1 sentinel (10k items) time: 0.019
    -1 sequential (10k items) time: 0.022
    -1 binary (10k items) time: 0
    -1 tabular (10k items) time: 0.002
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    executando com 100000 dados
    -=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    99999 avl (100k items) time: 0
    99998 sentinel (100k items) time: 0.175
    99998 sequential (100k items) time: 0.228
    99998 binary (100k items) time: 0.001
    99998 tabular (100k items) time: 0.021

```