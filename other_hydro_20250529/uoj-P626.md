<p>����һ�� $n$ ���� $m$ ���ߵ�����ͼ $G$ (����� $1 \sim n$ ���)�����庯�� $f(u, G)$ :</p>
<ol>
<li>��ʼ������ֵ $cnt = 0$��ͼ $G�� = G$��</li>
<li>�� $1$ �� $n$ ��˳��ö�ٶ��� $v$�������ǰ��ͼ $G��$ �У��� $u$ �� $v$ ��� $v$ �� $u$ ��·�������ڣ��� $cnt + 1$������ͼ $G��$ ��ɾȥ���� $v$ �Լ�������صıߡ�</li>
<li>�� $2$ �������󣬷���ֵ $cnt$ ��Ϊ����ֵ��</li>
</ol>
<p>���ڸ���һ������ͼ G,������� $h(G) = f(1, G) + f(2, G) + \dots + f(n, G)$ ��ֵ��</p>
<p>����һ���أ���ɾ����������˳������ģ��� $1 \sim i$ ���ߺ��ͼΪ $G_i (1 \leq i \leq m)$������������� $h(G_i)$ ��ֵ��</p>
<h2>�����ʽ</h2>
<p>��һ���������� $n, m$ ��ʾͼ�ĵ����������</p>
<p>������ $m$ ��ÿ�������������� $i$ �е��������� $x_i, y_i$ ��ʾһ������� $x_i \rightarrow y_i$��</p>
<p>���ݱ�֤ $x_i \neq y_i$ ��ͬһ���߲��������Ρ�</p>
<h2>�����ʽ</h2>
<p>���һ�� $m + 1$ �����������е�һ������ʾ����������ͼ $G$ �� $h(G)$ ֵ���� $i (2 \leq i \leq m + 1)$ ��������ʾ $h(G_{i-1})$��</p>


<pre><code class="language-input1">4 6
2 3
3 2
4 1
1 4
2 1
3 1
</code></pre>


<pre><code class="language-output1">6 5 5 4 4 4 4
</code></pre>


<p>���ڸ���������ͼ $G$:</p>
<ol>
<li>$f (1, G) = 1$��������ɾ���˶��� $1$��</li>
<li>$f (2, G) = 1$��������ɾ���˶��� $2$��</li>
<li>$f (3, G) = 2$��������ɾ���˶��� $2, 3$��</li>
<li>$f (4, G) = 2$��������ɾ���˶��� $1, 4$��</li>
</ol>
<h2>������</h2>
<p>�������ļ��� <code>ex_graph2.in</code> �� <code>ex_graph2.ans</code>��</p>
<h2>������Լ��</h2>
<p>�������в������ݣ�$2 \leq n \leq 1000, 1 \leq m \leq 2 \times 10^5, 1 \leq x_i, y_i \leq n$��</p>
<p>ÿ�����Ե�ľ������Ƽ��±�:</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$n \leq$</th>
<th style="text-align:center;">$m \leq$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 11$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$2000$</td>
</tr>
<tr>
<td style="text-align:center;">$12 \sim 20$</td>
<td style="text-align:center;" rowspan="2">$1000$</td>
<td style="text-align:center;">$5000$</td>
</tr>
<tr>
<td style="text-align:center;">$21 \sim 25$</td>
<td style="text-align:center;">$2 \times 10^5$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./21027/file/attachment.zip">������������</a></p>
