<p>����һ�� $n$ ���� $m$ ���ߵ�����ͼ $G$���䶥��� $1 \sim n$ ��š�</p>
<p>�������������� $u, v$�����Ӷ��� $1$ �������ﶥ�� $v$ ������·������Ҫ�������� $u$����ƶ��� $u$ ֧�䶥�� $v$���ر�أ�ÿ������֧��������</p>
<p>��������һ���� $v$�����ǽ�ͼ��֧�䶥�� $v$ �Ķ��㼯�ϳ�Ϊ $v$ ����֧�伯 $D_v$��</p>
<p>������ $q$ �λ��������ѯ�ʣ�ÿ��ѯ�ʸ���һ������ߣ�����ش���ͼ $G$ �м�������ߺ��ж��ٸ��������֧�伯�����˱仯��</p>
<h2>�����ʽ</h2>
<p>��һ���������� $n, m, q$���ֱ��ʾͼ�еĶ��������������Լ�ѯ������</p>
<p>������ $m$ ��ÿ���������� $x_i, y_i$����ʾһ������� $x_i \rightarrow y_i$��</p>
<p>������ $q$ ��ÿ���������� $s_i, t_i$����ʾÿ��ѯ�ʼ���ı� $s_i \rightarrow t_i$��</p>
<p>���ݱ�֤������ͼ $G$ �У��� $1$ �ŵ�����ܵ������������㣬����ͼ�в������ر����Ի���</p>
<h2>�����ʽ</h2>
<p>����ÿ��ѯ�����һ��һ��������ʾ�𰸡�</p>


<pre><code class="language-input1">6 6 3
1 2
1 3
3 4
4 5
2 6
4 1
5 6
3 2
2 4
</code></pre>


<pre><code class="language-output1">1
0
2
</code></pre>


<p>����ԭͼ�����������֧�伯�ֱ�Ϊ��$D_1 = \{1\}, D_2 = \{1, 2\}, D_3 = \{1, 3\}, D_4 = \{1, 3, 4\}, D_5 = \{1, 3, 4, 5\}, D_6 = \{1, 2, 6\}$ ��</p>
<p>���� $5 \rightarrow 6$ ��$D_6 = \{1, 6\}$����������֧�伯���䡣</p>
<p>���� $3 \rightarrow 2$ ��û�е���֧�伯�ı䡣</p>
<p>���� $2 \rightarrow 4 $ �� $D_4 = \{1, 4\}, D_5 = \{1, 4, 5\}$����������֧�伯���䡣</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_dominator2.in</code> �� <code>ex_dominator2.ans</code>��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_dominator3.in</code> �� <code>ex_dominator3.ans</code>��</p>
<h2>������Լ��</h2>
<p>�������в������ݣ�$1 \leq n \leq 3000, 1 \leq m \leq 2 \times n, 1 \leq q \leq 2 \times 10^4$��</p>
<p>ÿ�����Ե�ľ������Ƽ��±�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$n \leq$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 6$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$q \leq 100$</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 9$</td>
<td style="text-align:center;" rowspan="2">$1000$</td>
<td style="text-align:center;">$m = n - 1$</td>
</tr>
<tr>
<td style="text-align:center;">$10 \sim 15$</td>
<td style="text-align:center;">$q \leq 1000$</td>
</tr>
<tr>
<td style="text-align:center;">$16 \sim 20$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">��</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./21031/file/attachment.zip">������������</a></p>
