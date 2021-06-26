---


---

<p><a href="../Summary.md">Voltar</a></p>
<h1>Quick Sort
</h1><h2 id="funcionamento">Funcionamento</h2>
<p>O quicksort adota a estratégia de divisão e conquista. A estratégia consiste em rearranjar as chaves de modo que as chaves "menores" precedem as chaves "maiores". Em seguida o quicksort ordena as duas sublistas de chaves menores e maiores recursivamente até que a lista completa se encontre ordenada.</p>
<h2 id="exemplo-de-implementação">Exemplo de Implementação</h2>
<pre><code>import java.io.*;

class GFG{

  

static void swap(int[] arr, int i, int j){
int temp = arr[i];
arr[i] = arr[j];
arr[j] = temp;
}

/* Esta função pega o último elemento como pivô, coloca
o elemento pivô em sua posição correta na classificação
array e coloca todos menores (menores que pivô)
à esquerda do pivô e todos os elementos maiores à direita do pivô */

static int partition(int[] arr, int low, int high){

	// pivot
	int pivot = arr[high];

	// Índice de elemento menor e indica a posição certa do pivô encontrado até agora
	int i = (low - 1);

	for(int j = low; j &lt;= high - 1; j++){
		// Se o elemento atual for menor do que o pivô
		if (arr[j] &lt; pivot){
			i++;
			swap(arr, i, j);
		}
	}

	swap(arr, i + 1, high);

	return (i + 1);

	}
	
static void quickSort(int[] arr, int low, int high){

	if (low &lt; high)	{

		// pi é o índice de particionamento, arr [p] agora está no lugar certo
		int pi = partition(arr, low, high);

		// Classifica os elementos separadamente antes da partição e depois da partição
		quickSort(arr, low, pi - 1);

		quickSort(arr, pi + 1, high);

		}

	}

	// Imprimir

static void printArray(int[] arr, int size){

		for(int i = 0; i &lt; size; i++)

		System.out.print(arr[i] + " ");

		System.out.println();

	}

// Teste

public static void main(String[] args){

		int[] arr = { 10, 7, 8, 9, 1, 5 };

		int n = arr.length;

		quickSort(arr, 0, n - 1);

		System.out.println("Sorted array: ");

		printArray(arr, n);

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
<td>4,507</td>
<td>176065</td>
<td>103635</td>
</tr>
</tbody>
</table>
