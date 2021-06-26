---


---

<p><a href="../Readme.md">Voltar</a></p>
<h1>Selection Sort
</h1><h2 id="funcionamento">Funcionamento</h2>
<p>É um algoritmo de ordenação baseado em passar sempre o menor valor do vetor para a primeira posição (ou o maior dependendo da ordem requerida), depois o de segundo menor valor para a segunda posição, e assim é feito sucessivamente com os elementos restantes, até os últimos dois elementos.</p>
<h2 id="exemplo-de-implementação">Exemplo de Implementação</h2>
<pre><code>class SelectionSort{

	void sort(int arr[]){
		int n = arr.length;
			// Limite de movimento um por um
			for (int i = 0; i &lt; n-1; i++){
				// Encontre o elemento mínimo em uma matriz
				int min_idx = i;
				for (int j = i+1; j &lt; n; j++){
					if (arr[j] &lt; arr[min_idx]){
						min_idx = j;
						// Troque o elemento mínimo encontrado pelo primeiro elemento
						int temp = arr[min_idx];
						arr[min_idx] = arr[i];
						arr[i] = temp;
						}
					}
				}
			}	
	// Mostrar os arrays
	void printArray(int arr[]){
		int n = arr.length;
		for (int i=0; i&lt;n; ++i){
			System.out.print(arr[i]+" ");
			System.out.println();
		}
	}
	
	// teste
	public static void main(String args[]){
		SelectionSort ob = new SelectionSort();
		int arr[] = {64,25,12,22,11};
		ob.sort(arr);
		System.out.println("Sorted array");
		ob.printArray(arr);
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
<td>545,1068</td>
<td>49995000</td>
<td>74237889</td>
</tr>
</tbody>
</table>
