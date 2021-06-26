---


---

<h1>Bubble Sort</h1>
<h2 id="funcionamento">Funcionamento</h2>
<p>É um método de ordenação flutuante, ou por bolha é uma dos algoritmos de ordenação mais simples, sua metodologia é percorrer o vector varias vezes e a cada passagem fazer o número maior para o topo da sequencia</p>
<h2 id="exemplo-de-implementação">Exemplo de Implementação</h2>
<pre><code>package bubblesort;

public class BubbleSort {

	public static void main(String args[]) {
		int[] v = {5, 2, 4, 3, 0, 9, 7, 8, 1, 6};
	BubbleSort bs = new BubbleSort();
	bs.ordenar(v);
	for(int num : v) {
		System.out.print(num + " ");
		}
	}

public void ordenar(int[] v) {
	// for utilizado para controlar a quantidade de vezes que o vetor será ordenado.
		for(int i = 0; i &lt; v.length - 1; i++) {
		
	// for utilizado para ordenar o vetor.
	for(int j = 0; j &lt; v.length - 1 - i; j++) {

	/* Se o valor da posição atual do vetor for maior que o próximo valor, então troca os valores de lugar no vetor. */
		if(v[j] &gt; v[j + 1]) {
			int aux = v[j];
			v[j] = v[j + 1];
			v[j + 1] = aux;
			}
		}
	}
}
</code></pre>
<h2 id="performance">Performance</h2>
<ol>
<li>Lista ordenada em ordem crescente.</li>
<li>Lista ordenada em ordem decrescente.</li>
<li>Lista desordenada com números aleatórios.</li>
</ol>

<table>
<thead>
<tr>
<th>Tipo Ordenação</th>
<th>Tamanho vetor</th>
<th>Tempo</th>
<th>Comparações</th>
<th>Movimentações</th>
</tr>
</thead>
<tbody>
<tr>
<td>1</td>
<td>100</td>
<td>0,0988</td>
<td>5050</td>
<td>0</td>
</tr>
<tr>
<td>1</td>
<td>1000</td>
<td>9,5415</td>
<td>500500</td>
<td>0</td>
</tr>
<tr>
<td>1</td>
<td>10000</td>
<td>934,5364</td>
<td>50005000</td>
<td>0</td>
</tr>
<tr>
<td>2</td>
<td>100</td>
<td>0,2045</td>
<td>5050</td>
<td>14850</td>
</tr>
<tr>
<td>2</td>
<td>1000</td>
<td>20,3377</td>
<td>500500</td>
<td>1498500</td>
</tr>
<tr>
<td>2</td>
<td>10000</td>
<td>1838,0272</td>
<td>50005000</td>
<td>149985000</td>
</tr>
<tr>
<td>3</td>
<td>100</td>
<td>0,1596</td>
<td>5050</td>
<td>6777</td>
</tr>
<tr>
<td>3</td>
<td>1000</td>
<td>16,6730</td>
<td>500500</td>
<td>756840</td>
</tr>
<tr>
<td>3</td>
<td>10000</td>
<td>1455,9734</td>
<td>50005000</td>
<td>74237889</td>
</tr>
</tbody>
</table>
