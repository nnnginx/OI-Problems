<p>UOI ���ڿ����ˣ�������Ҫ�Ա�׼������ͨ�������ѡ����̨�콱��</p>
<p>�����������һ��ѡ��һ���� $n$ �����ˡ�����׼ȷ��˵��������һȺ�Ի�·������ͬ�������۷䣬�ʶ��ڱ�����ȡ������ȫ��ͬ�ķ�����</p>
<p>����ͨ����ǳ�ǿ��һ���� $m$ �ַ��š����������Ա��ÿֻ�����۷������Ҫôֻ��Ҫһ�����ţ�Ҫôֻ��Ҫ�������š�</p>
<p>����Ҫ����һ��ѡ�ֱ�дһ��������������������ɵĻ��������ٰ�˳�������������������µ�����</p>
<ol>
<li>����Ե����� $n$ �����ֵ�����˳��</li>
<li>���������۷�������Ļ��������������ŵ�����������˳����ǵ����ָ���Ķ���ͬһֻ�۷䡣����������ÿ���������ŵ�������ȿ��԰�˳��дҲ���԰�����д��</li>
<li>���ܴ���������ͬ�Ķ�ֻ�۷䣬������ȻҪ��������ֶ�Ρ�</li>
</ol>
<p>Ϊ�˱��������ԣ���ϣ����������˳���������Ǹ����Ĵ���Ҳ����˵����Ҫ�����ִ�������ķ������д����Ҷ��ʹ��������û������</p>
<p><strong>�������ݱ�֤�н⡣</strong></p>
<h2>�����ʽ</h2>
<p>��һ������������ $n,m$���ֱ��ʾѡ�ָ����ͷ�������ѡ�ִ� $1 \ldots n$ ��š�</p>
<p>������ $n$ �У��� $i$ ��������һ�������� $l_i \in \{1,2\}$ ��ʾ $i$ ��ѡ�ֵ����ֳ��ȣ����� $l_i$ �� $1 \sim m$ �����������ʾ�� $i$ ���˵����֡�</p>
<h2>�����ʽ</h2>
<p>��һ������� $n$ �� $1\sim n$ ��������ɵ����У��� $i$ ��Ϊ $p_i$����ʾ��������ĵ� $i$ ��ѡ���� $p_i$ ��ѡ�֡�</p>
<p>��һ����� $n$ �� $01$ �������� $i$ ��Ϊ $0$ ��ʾ $p_i$ ��ѡ�ֵ���������д��������˳��һ�£���Ϊ $1$ ��ʾ����д��</p>
<p>ע�⣬��� $p_i$ ��ѡ�����ֳ���Ϊ $1$������������� $0$ �� $1$������ж��ֺϷ��Ļ�������������������һ����</p>


<pre><code class="language-input1">4 2
2 1 1
2 1 2
1 1
1 2
</code></pre>


<pre><code class="language-output1">4 1 3 2 
0 1 0 0
</code></pre>


<p>����һ�����Ӧ�Ļ��Ĵ��� $211112$��</p>


<pre><code class="language-input2">2 2
1 1
2 1 2
</code></pre>


<pre><code class="language-output2">1 2 
0 1
</code></pre>


<p>�����������Ӧ�Ļ��Ĵ��� $121$��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_namelist3.in</code> �� <code>ex_namelist3.out</code>�������������������� 5 �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_namelist4.in</code> �� <code>ex_namelist4.out</code>�������������������� 6 �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_namelist5.in</code> �� <code>ex_namelist5.out</code>�������������������� 5 �����ʡ�</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1\leq n,m\leq 5\times 10^5$���� $L=\sum_{i=1}^{n} l_i$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n,m\le$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="2">��</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$5\times 10^5$</td>
<td style="text-align:center;">$l_i=2$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;" rowspan="3">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">$5\times 10^5$</td>
<td style="text-align:center;">$L$ Ϊż��</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$L$ Ϊ����</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
