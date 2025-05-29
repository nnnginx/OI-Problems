<p>C ����һ�����ٲ�ʢ�Ĺ��ң����� $n$ �����к� $m$ �������·��ɣ����д� $1$ �� $n$ ��š������ $x$ �ų��г�����������������·���ܵ��� $y$ �ų��У���ô���ǳ� $x$ �ų��пɵ��� $y$ �ų��У����� $x \Rightarrow y$��C ���ĵ�·��һ���ص㣺������������ $x,~y,~z$���� $x \Rightarrow z$ �� $y \Rightarrow z$����ô�� $x \Rightarrow y$ �� $y \Rightarrow x$��</p>
<p>�ٹ�һ���¾��� C ��������ǧ������գ����� C �����������ڳﱸʢ���������䡣Ŀǰ C ����֪���������� $q$ �����мƻ����� $i$ ������ϣ���ӳ��� $s_i$ �������������ɸ����к��ڳ��� $t_i$ �������������й����У�<strong>һ�����п��Ա��������</strong>��Ϊ���������е���Ȥ��ÿ�����л�����ʱ�޽��� $k~(0 \leq k \leq 2)$ �������·ר�Ź���������ʹ�ã� ���������мƻ�����ͨ�����������޽��ĵ�·��</p>
<p>���� C ����֪����ÿ�����мƻ����ܻ�<strong>��������������</strong>��</p>
<p>ע�⣺��ʱ�޽����ĵ�·<strong>���Բ����� C ����·ԭ�е��ص�</strong>��</p>
<h2>�����ʽ</h2>
<p>��һ�а����ĸ����� $n,~m,~q,~k$���ֱ��ʾ����������·�������мƻ����Լ�ÿ��������ʱ�޽��ĵ�·���� </p>
<p>������ $m$ �У�ÿ�а����������� $u,~v$����ʾһ�������· $u \rightarrow v$��</p>
<p>������ $q$ �У�ÿ��ǰ�������� $s_i, t_i$����ʾÿ�����е�������յ㣻���н������� $k$ ������ $a,~b$��ÿ��������ʾһ����ʱ��ӵ������· $a \rightarrow b$��
���ݱ�֤���� C ��ԭ�е������·��Ϊ�����·�����г��п��Ի��</p>
<h2>�����ʽ</h2>
<p>����ÿ��ѯ�ʣ����һ��һ��������ʾ�𰸡����һ�����д��������޷������յ㣬��� $0$ ���ɡ�</p>


<pre><code class="language-input1">5 6 4 1
1 2
1 3
1 4
2 5
4 5
5 4
1 4 5 1
2 3 5 3
1 2 5 2
3 4 5 1
</code></pre>


<pre><code class="language-output1">4
4
4
0
</code></pre>


<p>��һ�μƻ������Ϊ $1$ �ŵ㣬�յ�Ϊ $4$ �ŵ㣬��ʱ�޽���·Ϊ $5 \rightarrow 1$�����տ��ܾ����ĳ��б��Ϊ ${1,~2,~4,~5}$��</p>
<p>�ڶ��μƻ������Ϊ $2$ �ŵ㣬�յ�Ϊ $3$ �ŵ㣬��ʱ�޽���·Ϊ $5 \rightarrow 3$�����տ��ܾ����ĳ��б��Ϊ ${2,~3,~4,~5}$��</p>
<p>�����μƻ������Ϊ $1$ �ŵ㣬�յ�Ϊ $2$ �ŵ㣬��ʱ�޽���·Ϊ $5 \rightarrow 2$�����տ��ܾ����ĳ��б��Ϊ ${1,~2,~4,~5}$��</p>
<p>���Ĵμƻ������Ϊ $3$ �ŵ㣬�յ�Ϊ $4$ �ŵ㣬��ʱ�޽���·Ϊ $5 \rightarrow 1$�����մ� $3$ �ŵ�����޷����� $4$ �ŵ㡣</p>
<h2>������</h2>
<p>�������ļ��� <code>celebration2.in</code> �� <code>celebration2.ans</code>��</p>
<p>������Լ������Ե� $5 \sim 7$ һ�¡�</p>
<h2>������</h2>
<p>�������ļ��� <code>celebration3.in</code> �� <code>celebration3.ans</code>��</p>
<p>������Լ������Ե� $10 \sim 11$ һ�¡�</p>
<h2>������</h2>
<p>�������ļ��� <code>celebration4.in</code> �� <code>celebration4.ans</code>��</p>
<p>������Լ������Ե� $15 \sim 16$ һ�¡�</p>
<h2>������</h2>
<p>�������ļ��� <code>celebration5.in</code> �� <code>celebration5.ans</code>��</p>
<p>������Լ������Ե� $20 \sim 25$ һ�¡�</p>
<h2>���Ե�Լ��</h2>
<p>���� $100\%$ �����ݣ��� $1\le n,~q \le 3\times 10^5,~$$n-1\le m\le 6\times 10^5,~$$0\le k\le 2$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">���Ե���</th>
<th style="text-align:center;">$n,~q\le$</th>
<th style="text-align:center;">$k$</th>
<th style="text-align:center;">��������</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$=0$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 7$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$\le 2$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$8 \sim 9$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=0$</td>
<td style="text-align:center;">$m=n-1$</td>
</tr>
<tr>
<td style="text-align:center;">$10 \sim 11$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=1$</td>
<td style="text-align:center;">$m=n-1$</td>
</tr>
<tr>
<td style="text-align:center;">$12 \sim 14$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=2$</td>
<td style="text-align:center;">$m=n-1$</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 16$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=0$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 19$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=1$</td>
<td style="text-align:center;">��</td>
</tr>
<tr>
<td style="text-align:center;">$20 \sim 25$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=2$</td>
<td style="text-align:center;">��</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\require{cancel}\cancel{\texttt{1s}}\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{1GB}$</strong></p>
