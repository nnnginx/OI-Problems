<p>�õ������й�����Ԯ���������������������лص�����������ܿ��£���˾ɲ�������ʤ����������������������������ȫ���������������ڣ�ʣ��һ���־������������������������ڼ�̵ı��������������翹��Ϊ�˹���������������������㡪������Ǳ����������̽�鱨��</p>
<p>Ȼ������Ǳ���ʱ��ץס�ˡ��㱻������������������ǰ�����������ҵ�����ѧ����С L������ʾ��Ҫ���ܺ�������Ϸ����ʤ�����ܷ����ߣ�һ�����λ��ᡣ</p>
<p>��һ�����ھ���ͼ�������� Hamilton ����С L ���ֻ�ʤ���ڶ����Ǹ�һ����С���Ϊ $k$ ������ͼ��һ�� $k$ �����������Ҫ��ͼ���ҳ� $k$ ���㣬ʹ����������ͼ�������������ɾ���� $k$ �����ͼ����ͨ�����ڹ��ڽ��ţ�������Ҫ��֤��ͨ��</p>
<p>���������һ�λ����ˣ�������ĿҲ��Ϊ���ӣ�</p>
<p>����һ��������ͼ $G$ �ǡ��������ģ����ҽ����� $G$ �������ĸ���ͬ�� $A,B,C,D$���� $AB,BC,CD$ ����бߣ��� $AC,BD,AD$ �䲻����ͬʱû�бߣ���Ҫô $AC$ �бߣ�Ҫô $BD$ �бߣ�Ҫô $AD$ �бߣ���</p>
<p><img src="https://img.uoj.ac/problem/632/632.png" alt="����" class="img-responsive center-block" style="width:400px;"></p>
<p>��������ͼƬ��ߵ�ͼ�ǡ��������ģ����ұߵ�ͼ��ȡ $A=1,B=2,C=4,D=5$ ���� $AB,BC,CD$ ����бߣ��� $AC,BD,AD$ ���û�бߣ���˲���һ������������ͼ��</p>
<p>����һ�� $n$ ����ġ��������ļ�����ͼ $G$ ����Ҫ������ $i=1, \dots, n$����� $G$ ���ж��ٸ��㼯�Ӽ���������ͼͬ���� $K_i$������ $K_i$ ���� $i$ �������ȫͼ��Ҳ����˵����������һ�� $i$���㶼Ҫ��� $G$ ���ж��ٸ���СΪ $i$ �ĵ�ļ��ϣ�ʹ�ü���������������� $G$ ����ֱ�ӵı���������ֻ��Ҫ�������������𰸶� $998244353$ ȡģ��ֵ��</p>
<p>���׷��֣�������ⲻ��ȼ��� $G$ ������Ŵ�С���ס�</p>
<p>�㷢��������������ǿ϶����������ģ����������������ṩ��һ̨�����������Ҫ�ü�����������</p>
<p><strong>��ʾ����ֻ��Ҫ������������⣬ǰ���������뱾��û���κι�ϵ</strong>��</p>
<h2>�����ʽ</h2>
<p><strong>Ϊ�˼�С����������������������ѹ��</strong>��</p>
<p>��һ��һ�������� $n$����ʾһ������������ͼ $G$ �ĵ�����</p>
<p>������ $n-1$ �У��� $i$ ��Ϊһ������Ϊ $\lceil \frac{n-i}{4} \rceil$ ���ַ����������� <samp>'0'</samp> ~ <samp>'9'</samp> �� <samp>'A'</samp> ~ <samp>'F'</samp>������ַ� <samp>'0'</samp>~<samp>'9'</samp> ���ζ�Ӧ���� $0\sim 9$��<samp>'A'</samp>~<samp>'F'</samp> ���ζ�Ӧ���� $10\sim 15$�� </p>
<p>�� $\forall 1\leq j\leq n-i$��$G$ �б� $(i,i+j)$ ���ڵ��ҽ������ַ����� $\lceil \frac{j}{4} \rceil$ ���ַ�����Ӧ�����Ķ����Ʊ�ʾ�´ӵ����ߵ� $(j-1) \bmod 4$ λΪ $1$��ע���� $(n-i) \bmod 4\neq 0$�������һ���ַ������Ʊ�ʾ��û�ж����λһ��Ϊ $0$��</p>
<h2>�����ʽ</h2>
<p>���һ�� $n$ ���ÿո�ֿ����������� $i$ ������Ϊ $G$ �㼯�Ӽ���������ͼ��ͬ���� $K_i$ �ĸ����� $998244353$ ȡģ��ֵ��</p>


<pre><code class="language-input1">4
5
1
1
</code></pre>


<pre><code class="language-output1">4 4 0 0
</code></pre>


<p>�������ѹ�󣬵õ��� $G$ ���ڽӾ���Ϊ</p>
<pre>0101
1010
0101
1010
</pre>

<p>����һ�� $4$ ����Ļ����б� $(1,2),(2,3),(3,4),(4,1)$��������ͼΪ��Ŀ����ͼƬ�е���ͼ��</p>
<p>���׿�����������Ŵ�СΪ $2$���Ҹ��� $4$ ���㼯�Ӽ���������ͼ�� $K_1$ �� $K_2$���� $4$ ������ $4$ ���ߡ�</p>


<pre><code class="language-input2">10
FF1
FF
F7
F3
F1
F
7
3
1
</code></pre>


<pre><code class="language-output2">10 45 120 210 252 210 120 45 10 1
</code></pre>


<p>����һ�� $10$ �������ȫͼ���� $K_{10}$�������������������� $2$ �����ơ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_clique3.in</code>�� <code>ex_clique3.out</code>�������������������� $3$ �����ơ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_clique4.in</code>�� <code>ex_clique4.out</code>��</p>
<h2>���ݷ�Χ</h2>
<p>�����������ݣ� $2\leq n\leq 8000$ ���� $m$ Ϊ $G$ �б������� $0\leq m\leq \frac{n(n-1)}{2}$����֤����� $G$ �ǡ��������ġ� </p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$1000$</td>
<td style="text-align:center;">$m=\frac{n(n-1)}{2}$</td>
<td>$5$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$m\geq \frac{n(n-1)}{2}-20$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">��</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$4000$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$8000$</td>
<td style="text-align:center;">$30$</td>
</tr>
</tbody>
</table>
</div>
<p>�������� A: $G$ ��һ����ȫ $k$ ��ͼ���� $\exists 1\leq k\leq n$ ��ʹ $G$ �㼯���Ա�����Ϊ $k$ ���ǿռ��ϣ�������֮���бߵ��ҽ������ǲ���ͬһ�����С�</p>
<p><strong>ʱ������</strong>��$2\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$1\texttt{GB}$</p>
<h2>��ʾ</h2>
<p><strong>��ѡ�������Լ��㷨�ĳ������������Ч��</strong>��</p>
<h2>����</h2>
<p><a href="./21033/file/attachment.zip">������������</a></p>
