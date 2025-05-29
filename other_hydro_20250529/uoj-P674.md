<p>С L ��һ������ͼ��ͼ�еĶ�����Է�Ϊ $k$ �㣬�� $i$ ���� $n_i$ �����㣬�� $1$ ����� $k$ ��<strong>��������ͬ</strong>���� $n_1=n_k$���Ҷ��ڵ� $j$��$2 \leq j \leq k-1$�� �㣬$n_1 \leq n_j \leq 2n_1$�����ڵ� $j$��$1 \leq j &lt; k$�� ��Ķ��㣬������Ϊ���ı�ֻ������� $j+1$ ��Ķ��㡣û�б������ $1$ ��Ķ��㣬�� $k$ ��Ķ��㲻���������������ߡ�</p>
<p>����С L Ҫ�����ͼ��ѡ�� $n_1$ ��·����ÿ��·���Ե� $1$ �㶥��Ϊ��㣬�� $k$ �㶥��Ϊ�յ㣬��Ҫ��<strong>ͼ�е�ÿ���������������һ��·����</strong>��������أ���ÿһ�㶥�㰴�� $1, 2, \cdots, n_i$ ���б�ţ���ÿ��·������дΪһ�� $k$ Ԫ�� ����ʾ����·�����ξ����� $j$ ��� $p_j$��$1 \leq p_j \leq n_j$���Ŷ��㣬���ҵ� $j$��$1 \leq j &lt; k$����� $p_j$ �Ŷ�����һ��������� $j+1$ ��ĵ� $p_{j+1}$ �Ŷ��㡣</p>
<p>С L ����Щ·��������ֽ�ϣ��������ǻ�������ɸ����㡣��������·�� $P, Q$���ֱ��������ڵ� $j$ ����� $j+1$ ��֮�������Ϊ $(P_j, P_{j+1})$ �� $(Q_j, Q_{j+1})$������</p>
<p>$$(P_j-Q_j) \times (P_{j+1}-Q_{j+1}) &lt; 0$$</p>
<p>��������ڵ� $j$ ��������һ�����㡣����·���Ľ�����Ϊ�����ڵ� $1, 2, \cdots, n$ �������Ľ�����������������·�����������Ľ�����Ϊ <strong>������ͬ·���佻����֮��</strong> ��������ͼ��һ�� $3$ ��·������ $3$ ����������ӣ����к�ɫ���ǽ��㡣</p>
<p><img src="https://img.uoj.ac/problem/674/1.png" alt="����" class="img-responsive center-block"></p>
<p>С L ������֪����ż���������·�����������������������·������������ٸ�������·����������Ϊ��ͬ�ģ����ҽ������ǵ� $n_1$ ��·������һ�������˳��д�µ� $k$ Ԫ���ܶ�Ӧ��ͬ���������Ľ�����ܴܺ������������ $998244353$��һ����������ȡģ���ֵ��</p>
<h2>�����ʽ</h2>
<p>�����ж������ݣ��������ݵ�һ��һ�������� $T$����ʾ��������������ÿ�����ݣ�</p>
<p>��һ��һ�������� $k$����ʾһ���� $k$ �㶥�㡣</p>
<p>�ڶ��а��� $k$ ������ $n_1, n_2, \cdots, n_k$�����α�ʾÿһ��Ķ�����������֤ $n_1=n_k$���� $n_1 \leq n_i \leq 2n_1$��$2 \leq i \leq k-1$����</p>
<p>�����а��� $k-1$ ������ �����α�ʾ�� $j$ �㶥�㵽�� $j+1$ �㶥��ı�������֤ $m_j \leq n_j \times n_{j+1}$��</p>
<p>�������� $k-1$ �����롣�� $j$��$1 \leq j &lt; k$����������� $m_j$ �У�ÿһ���������� $u, v$����ʾ�� $j$ ��� $u$ �Ŷ�����һ��������� $j+1$ ��� $v$ �Ŷ��㡣</p>
<p>���ݱ�֤ͼ�в�������رߡ�</p>
<h2>�����ʽ</h2>
<p>����� $T$ �У�ÿ��һ����������ʾ�������ݵĴ𰸶� $998244353$ ȡģ���ֵ��</p>


<pre><code class="language-input1">1
3
2 3 2
4 4
1 1 
1 2
2 1
2 3
1 2
2 1
3 1
3 2
</code></pre>


<pre><code class="language-output1">1
</code></pre>


<p>ż��������ķ����� $2$ ��������������ķ����� $1$ �������Դ�Ϊ $1$��</p>
<p>���±���·�� $1$ ��·�� $2$ �ķ�������������õ���ͬ�ķ���������·�� $1$ Ϊ $(2, 3, 1)$ ��·�� $2$ Ϊ $(1, 1, 2)$ �ķ����뷽�� $1$ ����ͬ�ķ��������Բ��ᱻ����𰸡�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">·������</th>
<th style="text-align:center;">·�� $1$</th>
<th style="text-align:center;">·�� $2$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$(1, 1, 2)$</td>
<td style="text-align:center;">$(2, 3, 1)$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$(1, 2, 1)$</td>
<td style="text-align:center;">$(2, 1, 2)$</td>
<td style="text-align:center;">$2$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$(1, 2, 1)$</td>
<td style="text-align:center;">$(2, 3, 2)$</td>
<td style="text-align:center;">$0$</td>
</tr>
</tbody>
</table>
</div>
<h2>����������������������</h2>
<p>�������ļ����ء�</p>
<h2>���ݷ�Χ</h2>
<p>�������в������ݣ�$2 \leq k \leq 100$��$2 \leq n_1 \leq 100$��$1 \leq T \leq 5$��</p>
<p>ÿ�����Ե��У���֤ $n_1 &gt; 10$ ������ֻ�� $1$ �顣</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$k=$</th>
<th style="text-align:center;">$n_1\leq$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$10$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 6$</td>
<td style="text-align:center;" rowspan="3">$10$</td>
<td style="text-align:center;">A,B</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 8$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 10$</td>
<td style="text-align:center;" rowspan="2">��</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 13$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$100$</td>
</tr>
<tr>
<td style="text-align:center;">$14 \sim 15$</td>
<td style="text-align:center;" rowspan="3">$100$</td>
<td style="text-align:center;">A,B</td>
</tr>
<tr>
<td style="text-align:center;">$16 \sim 17$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$18 \sim 20$</td>
<td style="text-align:center;">��</td>
</tr>
</tbody>
</table>
</div>
<p>�������� A���������� $i$��$2 \leq i \leq k-1$������ $n_i=n_1$��</p>
<p>�������� B����֤·��������������Ϊ $1$��</p>
<p><strong>ʱ������: $\require{cancel}\cancel{\texttt{1s}}\texttt{2s}$</strong></p>
<p><strong>�ռ�����: $\texttt{1GB}$</strong></p>
