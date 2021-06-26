---


---

<p><a href="../Summary.md">Voltar</a></p>
<h1>Insertion Sort
</h1><h2 id="funcionamento">Funcionamento</h2>
<p>É um algoritmo de ordenação que constrói uma matriz final com um elemento de cada vez, uma inserção por vez. Assim é bastante eficiente para problemas com pequenas entradas, sendo o mais eficiente entre os algoritmos desta ordem de classificação..</p>
<h2 id="exemplo-de-implementação">Exemplo de Implementação</h2>
<pre><code>class InsertionSort {

void sort(int arr[]){
		int n = arr.length;
			for (int i = 1; i &lt; n; ++i) {
			int key = arr[i];
			int j = i - 1;
	  
		/* Mova os elementos de arr [0..i-1], que são
		maior que a chave, para uma posição à frente de
		sua posição atual */
		
		while (j &gt;= 0 &amp;&amp; arr[j] &gt; key) {
			arr[j + 1] = arr[j];
			j = j - 1;
			}
		arr[j + 1] = key;
		}
	}
	  
	//imprimir um array de tamanho n
	static void printArray(int arr[]){
		int n = arr.length;
		for (int i = 0; i &lt; n; ++i){
			System.out.print(arr[i] + " ");
			System.out.println();
		} 
	}
	// Teste
	public static void main(String args[]){
		int arr[] = { 12, 11, 13, 5, 6 };
		  
		InsertionSort ob = new InsertionSort();
		ob.sort(arr);
		printArray(arr);
	}
}
</code></pre>
<h2 id="performance">Performance</h2>
<p>Lista desordenada com números aleatórios.</p>

<table>
<thead>
<tr>
<th>Tamanho vetor</th>
<th>Tempo</th>
<th>Comparações</th>
<th>Movimentações</th>
</tr>
</thead>
<tbody>
<tr>
<td>10000</td>
<td>539,681</td>
<td>9999</td>
<td>24765961</td>
</tr>
</tbody>
</table>
