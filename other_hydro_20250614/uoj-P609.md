<p>��սǰ�����й����ط��֣�ũҵ������С���Ұǧ��츮֮������������ũҵ�����й���һ��֧����ҵ����������ս�Һ����й�����������ˮ����ʧ�������ܵ������ƻ�����ʳ�;������������󽵵͡��������й�ũҵ����Ϊ���й���һ��Ҫ������⡣</p>
<p>���ؾ�����������ĸ��¼�����������������������⡣�������һ��֪�����ϣ�һ���ܶ�������������С��Ķ��һǧ�ˡ���ʹ������й��Ķ������������������Ҳ���Լ����������������</p>
<p>���ǽ���������ܵ���ʹ�ã�ֻ�ܼ��뵽һ�������ķ����л��ʹ�á�ͬʱ��������������ż�ǿ������ԣ���һ��ԭ�еķ��Ϸ���������Ϊ<strong>����</strong> $x$ ���򽫽�����������к󣬻����һ���Ķ����������ֵ�� $[0,m]$ ��ȸ�������������µķ��Ϸ������Ϊ $[x,x+m]$ ֮��ĵȸ������<strong>ʵ��</strong>������ $m$ ��һ��������<strong>����</strong>��</p>
<p>���ڷ���������½���������ܣ��������������� $n$ ����ϣ�����������ֱ�������У���ͬ���ϼ�������������������Ķ������������ء���ϣ�����ܸ����������յõ��ķ��Ϸ����������� $1\sim n$ С�ķ�������ֵ�ֱ��Ƕ��١�����֤������Ŀ�����������£�����ֵ��һ�������� $\frac{p}{q}$ ���� $q$ ���� $998244353$ �ı�������ֻ��Ҫ��� $p \cdot q^{-1} \bmod 998244353$ ��ֵ���ɡ�</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n,m$ ���ֱ��ʾ�����������ͽ�����ķ������ޡ�</p>
<p>������һ�� $n$ ������������ $i$ �������� $a_i$ ��ʾ�� $i$ ����ϵķ�����</p>
<h2>�����ʽ</h2>
<p>��� $n$ �У��� $i$ ��һ���Ǹ�������ʾ�� $i$ С�ķ�������ֵ�� $998244353$ ȡģ���ֵ��</p>


<pre><code class="language-input1">3 1
1 2 3
</code></pre>



<pre><code class="language-output1">499122178
499122179
499122180
</code></pre>



<p>������ϵķ����ֱ��� $a_1=1,a_2=2,a_3=3$ ���� $m=1$ ��</p>
<p>���׷��ֲ��۽���������Ķ�������Ƕ��٣����յõ���������Ϸ��� $b_i$ ��Ȼ���� $b_1\leq b_2\leq b_3$ ����˵� $i$ С���Ϸ�������ֵ��Ϊ $b_i$ ����ֵ $\frac{3}{2},\frac{5}{2},\frac{7}{2}$ ���� $998244353$ ȡģ�󼴵õ����������</p>


<pre><code class="language-input2">5 3
3 4 2 3 5
</code></pre>



<pre><code class="language-output2">505489582
791406484
246480092
249971894
702262855
</code></pre>


<h2>������</h2>
<p>�������ļ��� <code>ex_fertilizer3.in</code> �� <code>ex_fertilizer3.out</code> ��</p>
<h2>������</h2>
<p>�������ļ��� <code>ex_fertilizer4.in</code> �� <code>ex_fertilizer4.out</code> ��</p>
<h2>���ݷ�Χ</h2>
<p>�����������ݣ� $1\leq n\leq 2000,1\leq m,a_i\leq 10^8$ ��</p>
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
<td style="text-align:center;" rowspan="2">$2000$</td>
<td style="text-align:center;">$\forall 1\leq i &lt; n,a_i+m\leq a_{i+1}$</td>
<td style="text-align:center;">$3$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$\forall 1\leq i &lt; n,a_i=a_{i+1}$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;" rowspan="5">��</td>
<td style="text-align:center;">$16$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$80$</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$400$</td>
<td style="text-align:center;">$14$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$1500$</td>
<td style="text-align:center;">$23$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$8$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ������</strong>��$4\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./21013/file/attachment.zip">������������</a></p>
