<p>����һ�� $n$ ���� $2 m$ ���ߵ�����ͼ��ͼ�е�ÿ�����϶���һ����ǣ�����һ�������Ż��������š����� $k$ �ֲ�ͬ���������ͣ���ͼ�п����� $2 k$ �ֲ�ͬ�ı�ǡ��㡢�ߡ������������ $1$ ��ʼ��š�</p>
<p>ͼ�е�ÿ���߶������һ���߳ɶԳ��֡�������أ���ͼ�д���һ�����е� $w$ �����ŵ������ŵı� $(u, v)$����ͼ��һ������һ�����е� $w$ �����ŵ������ŵı� $(v, u)$��ͬ���أ�ͼ��ÿ�����������ŵı߽���Ӧ��һ��������ı���ͬ���������ŵıߡ�</p>
<p>�������������ͼ�й��ж��ٸ���� $(x, y)$��$1 \le x &lt; y \le n$�����㣺ͼ�д���һ���� $x$ �������� $y$ ��·�����Ұ�����˳��·���������ϵı��ƴ�ӵõ����ַ�����һ���Ϸ����������С�</p>
<h2>�����ʽ</h2>
<p>��һ���������� $n, m, k$���ֱ��ʾͼ�еĵ������߶�����������������</p>
<p>������ $m$ �У�ÿ���������� $u, v, w$����ʾһ���� $u$ �� $v$ ������ߣ�����Ϊ�� $w$ �����ŵ������ţ��Լ�һ���� $v$ �� $u$ ������ߣ�����Ϊ�� $w$ �����ŵ������š�</p>
<p>���������ͼ�У�����������ͬ�Ķ��������ж����������������ͼ�в������������������ߣ��� $u \ne v$��</p>
<h2>�����ʽ</h2>
<p>�����һ��һ����������ʾ���������ĵ��������</p>


<pre><code class="language-input1">4 5 1
4 3 1
4 1 1
4 2 1
1 3 1
2 1 1
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>���������ĵ�Լ����Ӧ��·��Ϊ��</p>
<p> $(1, 2)$��$1 \to 3 \to 4 \to 1 \to 2$��  </p>
<p> $(1, 4)$��$1 \to 3 \to 4$��  </p>
<p> $(2, 4)$��$2 \to 1 \to 4$��</p>


<pre><code class="language-input2">6 8 2
6 1 2
3 5 1
1 2 2
5 1 2
3 6 2
4 3 1
6 2 2
3 2 1
</code></pre>


<pre><code class="language-output2">10
</code></pre>

<h2>������</h2>
<p>�������ļ��� <code>ex_bracket3.in</code> �� <code>ex_bracket3.ans</code>��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_bracket4.in</code> �� <code>ex_bracket4.ans</code>��</p>
<h2>������Լ��</h2>
<p>�������в��Ե㣺$1 \le n \le 3 \times {10}^5$��$1 \le m \le 6 \times {10}^5$��$1 \le k, u, v \le n$��$1 \le w \le k$��</p>
<p>ÿ�����Ե�ľ������Ƽ��±�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$n =$</th>
<th style="text-align:center;">$m \le$</th>
<th style="text-align:center;">$k \le$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="2">$2$</td>
<td style="text-align:center;" rowspan="3">��</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 8$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 12$</td>
<td style="text-align:center;" rowspan="2">$3000$</td>
<td style="text-align:center;">$6000$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 16$</td>
<td style="text-align:center;" rowspan="2">$n - 1$</td>
<td style="text-align:center;" rowspan="3">$n$</td>
<td style="text-align:center;" rowspan="2">�����ڽ��ɴ������ű�ǵı߹��ɵĻ�</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 20$</td>
<td style="text-align:center;" rowspan="2">$3 \times {10}^5$</td>
</tr>
<tr>
<td style="text-align:center;">$21 \sim 25$</td>
<td style="text-align:center;">$6 \times {10}^5$</td>
<td style="text-align:center;">��</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./21005/file/attachment.zip">������������</a></p>
