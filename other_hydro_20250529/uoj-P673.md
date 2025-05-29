<p>С W ��һ�� $n$ �������������ϵ�ÿһ���߿�������߻����رߡ�����������Ҫ�������� $m$ �β����������в�����ʼǰ���������б߶�����ߡ��������������֣�</p>
<ol>
<li>���������� $a$ �� $b$�����ȶ��� $a$ �� $b$ ·���ϵ����е� $x$������ $a$ �� $b$������Ҫ���� $x$ ���������б߱�Ϊ��ߡ�Ȼ���ٽ� $a$ �� $b$ ·���ϰ��������б߱�Ϊ�رߡ�</li>
<li>���������� $a$ �� $b$������Ҫ���㵱ǰ $a$ �� $b$ ��·����һ�������������رߡ�</li>
</ol>
<h2>�����ʽ</h2>
<p>�����ж������ݣ��������ݵ�һ��һ�������� $T$����ʾ����������</p>
<p>����ÿ�����ݣ� ��һ�а����������� $n$ �� $m$������ $n$ ��ʾ���������$m$ ��ʾ����������</p>
<p>������ $n-1$ �У�ÿ�а����������� $u, v$����ʾ���ϵ�һ���ߡ�</p>
<p>������ $m$ �У�ÿ�а����������� $op_i, a_i, b_i$������һ������������ $op_i=1$ ��ʾ�� $1$ �������$op_i=2$ ��ʾ�� $2$ �������</p>
<p>���ݱ�֤ $a_i \neq b_i$��</p>
<h2>�����ʽ</h2>
<p>����ÿһ�ε� $2$ ����������һ��һ��������ʾ�𰸡�</p>


<pre><code class="language-input1">1
7 7
1 2
1 3
3 4
3 5
3 6
6 7
1 1 7
2 1 4
2 2 7
1 1 5
2 2 7
1 2 1
2 1 7
</code></pre>


<pre><code class="language-output1">1
3
2
1
</code></pre>


<p>�� 1 �β������ر��У�$(1, 3)$��$(3, 6)$��$(6, 7)$��</p>
<p>�� 2 �β������������ر��У�$(1, 3)$��</p>
<p>�� 3 �β������������ر��У�$(1, 3)$��$(3, 6)$��$(6, 7)$��</p>
<p>�� 4 �β��������� $(1, 3)$��$(3, 6)$ ��Ϊ��ߣ�֮�� $(1, 3)$��$(3, 5)$ ��Ϊ�رߡ�</p>
<p>�� 5 �β������������ر��У�$(1, 3)$��$(6, 7)$��</p>
<p>�� 6 �β��������� $(1, 3)$ ��Ϊ��ߣ�֮�� $(1, 2)$ ��Ϊ�رߡ�</p>
<p>�� 7 �β������������ر��У�$(6, 7)$��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_edge2.in</code> �� <code>ex_edge2.ans</code>��</p>
<p>������Լ������Ե� $3 \sim 6$ һ�¡�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_edge3.in</code> �� <code>ex_edge3.ans</code>��</p>
<p>������Լ������Ե� $9 \sim 10$ һ�¡�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_edge4.in</code> �� <code>ex_edge4.ans</code>��</p>
<p>������Լ������Ե� $11 \sim 14$ һ�¡�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_edge5.in</code> �� <code>ex_edge5.ans</code>��</p>
<p>������Լ������Ե� $17 \sim 20$ һ�¡�</p>
<h2>���Ե�Լ��</h2>
<p>�������в������ݣ��� $T \leq 3, 1 \leq n, m \leq 10^5$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$n, m \leq$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="2">��</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 6$</td>
<td style="text-align:center;">$5000$</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 8$</td>
<td style="text-align:center;" rowspan="3">${10}^5$</td>
<td style="text-align:center;">A, B</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 10$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 14$</td>
<td style="text-align:center;">B</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 16$</td>
<td style="text-align:center;">$2 \times 10^4$</td>
<td style="text-align:center;" rowspan="2">��</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 20$</td>
<td style="text-align:center;">${10}^5$</td>
</tr>
</tbody>
</table>
</div>
<p>�������� A��������̬��һ������</p>
<p>�������� B���� $2$ ����������� $a_i$ �� $b_i$ ֮���б�ֱ��������</p>
<p><strong>ʱ�����ƣ�$\require{cancel}\cancel{\texttt{1s}}\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{1GB}$</strong></p>
