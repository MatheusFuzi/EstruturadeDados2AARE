---


---

<p><img src="/img/unipar.png" alt="Alt text " title="teste"></p>
<div align="center"><b></b><h2>ADS - Análise e Desenvolvimento de Sistemas
<b><br><br>Estrutura de Dados 
<br><br>Métodos de Ordenação</b></h2></div>
<h2>Índice</h2>
<ul>
<li>
<h3>Questão 1</h3>
<ul>
<li>
<p>Métodos de Ordenação</p>
<ul>
<li><a href="#Conceito-M%C3%A9todos-de-Ordena%C3%A7%C3%A3o">Conceito geral</a></li>
<li><a href="Methods/BubbleSort.md">Bubble sort</a>
<ul>
<li><a href="Methods/BubbleSort.md#Funcionamento">Funcionamento</a></li>
<li><a href="Methods/BubbleSort.md#Performance">Performance</a></li>
<li><a href="Methods/BubbleSort.md#Exemplo-de-Implementa%C3%A7%C3%A3o">Exemplo de Implementação</a></li>
</ul>
</li>
<li><a href="Methods/SelectionSort.md">Selection sort</a>
<ul>
<li><a href="Methods/SelectionSort.md#Funcionamento">Funcionamento</a></li>
<li><a href="Methods/SelectionSort.md#Performance">Performance</a></li>
<li><a href="Methods/SelectionSort.md#Exemplo-de-Implementa%C3%A7%C3%A3o">Exemplo de Implementação</a></li>
</ul>
</li>
<li><a href="Methods/InsertionSort.md">Insertion sort</a>
<ul>
<li><a href="Methods/InsertionSort.md#Funcionamento">Funcionamento</a></li>
<li><a href="Methods/InsertionSort.md#Performance">Performance</a></li>
<li><a href="Methods/InsertionSort.md#Exemplo-de-Implementa%C3%A7%C3%A3o">Exemplo de Implementação</a></li>
</ul>
</li>
<li><a href="Methods/QuickSort.md">Quick sort</a>
<ul>
<li><a href="Methods/QuickSort.md#Funcionamento">Funcionamento</a></li>
<li><a href="Methods/QuickSort.md#Performance">Performance</a></li>
<li><a href="Methods/QuickSort.md#Exemplo-de-Implementa%C3%A7%C3%A3o">Exemplo de Implementação</a></li>
</ul>
</li>
</ul>
</li>
<li>
<p><a href="Methods/Conclusion.md">Conclusão</a></p>
</li>
</ul>
<h2 id="section"></h2>
</li>
<li>
<h3>Questão 2</h3>
<ul>
<li><a href="#Conceito-%C3%81rvore-Bin%C3%A1ria">Árvore binária</a>
<ul>
<li><a href="#Funcionamento-de-uma-%C3%81rvore-Bin%C3%A1ria">Funcionamento</a></li>
<li><a href="Methods/BinaryTree.md#Desempenho">Desempenho </a>
<ul>
<li><a href="Methods/BinaryTree.md#%C3%81rvore-Bin%C3%A1ria-Balanceada">Árvore binária balanceada</a></li>
<li><a href="Methods/BinaryTree.md#%C3%81rvore-Bin%C3%A1ria-N%C3%A3o-Balanceada">Árvore binária não balanceada</a></li>
<li><a href="Methods/BinaryTree.md#Impactos">Impactos na execução</a></li>
</ul>
</li>
<li><a href="Methods/BinaryTree.md#Exemplo">Exemplo</a></li>
</ul>
</li>
</ul>
</li>
</ul>
<br>
<h2 id="conceito-métodos-de-ordenaçãodiv">Conceito Métodos de Ordenação</h2>
<p>	A ordenação tem como objetivo organizar os dados listados em ordem crescente ou decrescente assim facilitando a recuperação destes dados em um determinado conjunto a que pertencem, deste modo auxiliando a busca e pesquisa dos dados.</p>
	<p>Imaginamos que em um sistema de contatos onde há vários contatos cadastrados, em uma busca geral retornando todos os contatos sem uma ordenação a procura pela informação que precisa fica lenta e inviável, com uma ordenação você consegue reduzir o tempo desta procura e facilitar a sua busca</p>
<h2 id="conceito-árvore-binária">Conceito Árvore Binária</h2>
<p>Uma árvore binária é uma estrutura de dados útil quando precisam ser tomadas decisões bidirecionais em cada ponto de um processo.</p>
<p>Por exemplo, suponha que precisemos encontrar todas as repetições numa lista de números. Uma maneira de fazer isto é comparar cada número com todos que o precedem.</p>
<h2 id="funcionamento-de-uma-árvore-binária">Funcionamento de uma Árvore Binária</h2>
<p>O primeiro número na lista é colocado num nó estabelecido como a raiz de uma árvore binária com as subárvores esquerda e direita vazias. Cada número sucessivo na lista é, então, comparado ao número na raiz. Se coincidirem, teremos uma repetição. Se for menor, examinaremos a subárvore esquerda; se for maior, examinaremos a subárvore direita.</p>
<p>Se a subárvore estiver vazia, o número não será repetido e será colocado num novo nó nesta posição na árvore. Se a subárvore não estiver vazia, compararemos o número ao conteúdo da raiz da subárvore e o processo inteiro será repetido com a subárvore.</p>

