<p>UOI �Ĺ����һЩ�������ص����Ǵ����ƶ��ģ����Դ�D�� AK ��Ҳ��׼�볡��</p>
<p>���ĵĴ�D�׾���Ԥ��һ������������ $n$ ������ѡ�ֵ�ˮƽ�����˽�ģ���γ���һ�ô�СΪ $n$ ���и��� $T$����Ϊ $1$����ʾ��D���Լ�����ڵ� $x$ �ĸ���Ϊ $\mathrm{fa}[x]$����֤ $\mathrm{fa}[x] &lt; x$��</p>
<p>���ݴ�D�׵Ľ�ģ��$\mathrm{fa}[x]$ ��ˮƽ���ϸ�� $x$ �ߵģ�����Ӧ������ǰ�档�����˵�����û��ô��ȷ���������������ͬһ����������˼ά��ʽ�ܽӽ������������ȽϺ���</p>
<p>��ʽ���أ����� $T$��������������һ�� <code>ddm</code> ���̣�����ȷ��ѡ�ֵĿ���������</p>
<ul>
<li>�ǰ�Ѿ����ǵĽڵ㼯��Ϊ $M$����ǰ���ڿ��ǵĽڵ�Ϊ $x$����ʼʱ $M=\{x\}$ �� $x=1$��</li>
<li>�ظ����¹���ֱ�����нڵ㶼�� $M$ �У�<ul>
<li>�� $x$ �����ж��Ӿ��� $M$ �У��� $x$ ��Ϊ $\mathrm{fa}[x]$��</li>
<li>������ѡһ�� $x$ δ������ $M$ �еĶ��� $u$���� $u$ ���� $M$ ���� $x$ ��Ϊ $u$��</li>
</ul>
</li>
</ul>
<p>ÿ�� <code>ddm</code> ���̶����Ӧһ�� <code>ddm</code> ��һ�� <code>ddm</code> ����һ�� $1\sim n$ ������ $p$������ $p_i$ ��ʾ�ڶ�Ӧ�� <code>ddm</code> �����У��ڵ� $i$ �ǵ� $p_i$ ������ $M$ �ġ���Ȼ�������� $T$�����ܻ��кܶ಻ͬ�� <code>ddm</code> ���̣���ȻҲ��Ӧ�ܶ಻ͬ�� <code>ddm</code> ��</p>
<p>����󣬴�D�׷�����ʵ����������һ�� $1\sim n$ ������ $a$�����ݴ�D�׵ķ������������ڿ��Ե�����Ա�֤�ġ�Ϊ��Բ��ȥ������Ҫ�ҵ��������һ���Ϸ� <code>ddm</code> �� $p$��ʹ�� $a$ ��ͨ�����·�ʽ���ɣ�</p>
<ul>
<li>��ʼ�� $b=p$��</li>
<li>��������β���ֱ�� $b=a$��<ul>
<li>��ѡ $x\ne 1$ ��ʹ�� $b[\mathrm{fa}[x]] &lt; b[x]$��Ȼ�󽻻� $b[\mathrm{fa}[x]]$ �� $b[x]$��</li>
</ul>
</li>
</ul>
<p>����ĳЩ���� $a$�����ܻ����û�кϷ� <code>ddm</code> ����������ʱ������Ҫ�����޽⡣</p>
<h2>�����ʽ</h2>
<p>��һ��һ������ $tp$����ʾ���Ե����ڵĲ��԰���š�</p>
<p>�ڶ���һ������ $n$����ʾ�� $T$ �ĵ�����</p>
<p>������ $n$ ���������� $i$ ��������ʾ $a_i$��</p>
<p>������ $n-1$ ���������� $i$ ��������ʾ $\mathrm{fa}[i+1]$ ���� $i+1$ �ĸ��ס�</p>
<h2>�����ʽ</h2>
<p>������ںϷ��� <code>ddm</code> �� $p$�����һ�� $n$ ���������� $i$ ��������ʾ $p_i$�����ڵ� $i$ �ڶ�Ӧ <code>ddm</code> �������ǵ� $p_i$ ������ $M$ �ģ�������ж���Ϸ��� $p$��������������һ����</p>
<p>������ֻ��Ҫ���һ�� <code>-1</code>��</p>


<pre><code class="language-input1">1
5
5 3 1 2 4
1 2 2 1
</code></pre>


<pre><code class="language-output1">1 2 3 4 5
</code></pre>


<p>�ǽ��� $b[\mathrm{fa}[x]],b[x]$ �Ĳ���Ϊ <code>swap(fa[x],x)</code>��</p>
<p>һ�ֿ��еĹ��� $a$ �ķ����ǣ� <code>swap(2,4), swap(1,2), swap(1,5), swap(2,3)</code>��</p>


<pre><code class="language-input2">1
8
8 3 5 7 1 2 4 6
1 1 1 3 1 3 4
</code></pre>


<pre><code class="language-output2">1 3 4 7 5 2 6 8
</code></pre>

<h2>������</h2>
<p>�������ļ��� <code>ex_tree3.in</code> �� <code>ex_tree3.out</code>�������������������� 2 �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_tree4.in</code> �� <code>ex_tree4.out</code>�������������������� 3 �����ʡ�</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_tree5.in</code> �� <code>ex_tree5.out</code>�������������������� 4 �����ʡ�</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ� $1\le n\le 10^5,1\le \mathrm{fa}[i] &lt; i$ ���ұ�֤ $a$ ��һ�� $1\sim n$ �����С�</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="3">$2000$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">B</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">$10^5$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">B</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p>�������� A ��� $x$ �ж�����ӿ�ѡ����Ϊ $u$ ʱѡ������С�Ĳ��Ե� <code>ddm</code> ���̶�Ӧ <code>ddm</code> �� $p_0$����ô�н⵱�ҽ��� $p_0$ �Ϸ���</p>
<p>�������� B ������ֻ��һ����Ķ��Ӹ��� $= 2$ ���Ҳ����ڶ��Ӹ��� $&gt;2$ �ĵ㡣���仰˵���� $T$ ����̬���� ���� Y�� �Ρ�</p>
<p><strong>ʱ�����ƣ�$\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
