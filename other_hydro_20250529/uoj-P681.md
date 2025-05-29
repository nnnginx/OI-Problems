<p>�����ҵ������������Ĺ���ʦ�ǣ���������������г������档</p>
<p>����ʦ����Ƴ���һ��ǳ���������桪����ǧ���档��������� $n$ ��������ɣ�ÿ��������һ�����Ĳ��� $a_i$��</p>
<p>�������� $x$ ���ٶ��н�ʱ��������ܹ���Ϊ $\oplus_{i=1}^n (a_i+x)$���� $(a_1 + x) \oplus (a_2 + x) \oplus \cdots \oplus (a_n + x)$������ $\oplus$ ��ʾ���</p>
<p>���ڷ��������� $m$ �ֲ�ͬ���ٶȣ�����Ҫ�����������Ĺ��ġ����ڷ��صı�Ƣ�������п�����Ҫ�õ�ÿһ���ٶȺ���������𰸡�</p>
<h2>�����ʽ</h2>
<p>��һ���������� $n, m, t$����ʾ���沿������ѯ�������Լ����ܲ�����</p>
<p>�ڶ��� $n$ ���������� $i$ ������ $a_i$ ��ʾ�����Ĺ��Ĳ�����</p>
<p>������ $m$ �У��� $i$ ������ $v'_i$����ʾ�� $i$ ��ѯ�ʵ��ٶ� $v_i=v'_i \oplus \left(t \times \left\lfloor\frac{\mathrm{lastans}}{2^{20}}\right\rfloor\right)$������ $\oplus$ ��ʾ���$\mathrm{lastans}$ ��ʾ��һ��ѯ�ʵ���������û����Ϊ $0$����</p>
<h2>�����ʽ</h2>
<p>��� $m$ �У��� $i$ ��һ������ $w_i$ ��ʾ�� $i$ ��ѯ�ʵĹ��ġ�</p>


<pre><code class="language-input1">2 2 0
1 2
2
3
</code></pre>


<pre><code class="language-output1">7
1
</code></pre>


<p>��һ��ѯ�ʵ����Ϊ $(1+2)\oplus(2+2)=3\oplus 4=7$��</p>
<p>��һ��ѯ�ʵ����Ϊ $(1+3)\oplus(2+3)=4\oplus 5=1$��</p>
<h2>����������</h2>
<p>���������ء�</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1\leq n, m\leq 2.5\times 10^5, t\in \{0, 1\}, 0\leq a_i,v'_i\lt 2^{60}$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n,m\leq$</th>
<th style="text-align:center;">$t=$</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">$10^3$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$2.5\times 10^5$</td>
<td style="text-align:center;">$0$</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$2.5\times 10^5$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{3s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
