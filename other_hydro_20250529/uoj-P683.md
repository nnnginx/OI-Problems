<p>�����ҵ��� skip �飬ϣ��������������վ��Ȼ��������֪��skip ����һֻ����ӡ��������ͳ��˿ڴ����Ӳ�ң��������ϰڳ���һ�ţ�Ҫ���غ�����һ����Ϸ��������Ϳ�ʼ�ɻ</p>
<p>��ʼʱÿöӲ��Ҫô���泯�ϣ�Ҫô���泯�ϡ���Ϸ��һ���ֽ��У����ĳһʱ�̣�������ʼʱ�̣�����Ӳ�Ҷ������棬����Ϸ���̽�����</p>
<p>ÿ�ֵĲ������£�</p>
<ol>
<li><p>ȡ��������Ӳ�ҡ�</p>
</li>
<li><p>�����öӲ�����泯�ϣ����� skip ��ѡ���Ƿ�ת�������ɷ���ѡ���Ƿ�ת��</p>
</li>
<li><p>����öӲ�ҷŵ����ұߡ�</p>
</li>
</ol>
<p>�����Ѿ�����·����Ū����ͷ�����������������ת��ÿ���ֵ�������ʱ����ѡ��ת�ĸ���Ϊ $p$��ѡ�񲻷�ת�ĸ���Ϊ $1-p$����ͬ��֮�������</p>
<p>skip ����һֻ�ǳ������ĸ��ӣ���ͨ�������ֶ�֪���˷��صĲ��ԣ��������������Ų��Ծ����Ƿ�ת��ʹ��Ϸ�����������������ܴ�</p>
<p>����Ϸ�������м��֣��𰸶� $998244353$ ȡģ��</p>
<h2>�����ʽ</h2>
<p>��һ��һ������Ϊ $n$ �� <samp>01</samp> ������ʾ��ʼ��Ӳ�����У�<samp>0</samp> ��ʾӲ�ұ��泯�ϣ�<samp>1</samp> ��ʾӲ�����泯�ϡ�</p>
<p>�ڶ����������� $a, b$����ʾ $p=\frac{a}{a+b}$��</p>
<h2>�����ʽ</h2>
<p>���һ����������ʾ skip ����ʹ�����Ų��Ե�����£���Ϸ��������Ҫ������������</p>
<p>�����Ϸ����������������������� $-1$��</p>
<p>������Ŀ���ݱ�֤�˸������ض�����д��һ������ $\frac{c}{d}$ ($c \ge 0, d \ge 1$)���ҷ�ĸ $d$ ���� $998244353$ �ı����������һ������ $x \in [0, 998244353)$ ʹ�� $dx$ �� $c$ ��ģ $998244353$ ������ͬ�ࡣ</p>


<pre><code class="language-input1">10
1 1
</code></pre>


<pre><code class="language-output1">8
</code></pre>


<p>������Ϊ <samp>10</samp> ʱ��skip ���ѡ��ת��Ϊ <samp>00</samp>��</p>
<p>��ʱ������ $\frac 12$ �ĸ��ʷ�תʹ�����Ϊ <samp>01</samp>��$\frac 12$ �ĸ��ʲ���תʹ���治�䣬���������ֺ�����Ϊ <samp>01</samp>��</p>
<p>������������ $\frac 12$ �ĸ��ʷ�תʹ��Ϸ������$\frac 12$ �ĸ��ʲ���תʹ�������±�Ϊ <samp>10</samp>��</p>
<p>��������������Ϊ <samp>10</samp> ʱ�������������ֺ���$\frac 12$ �ĸ�����Ϸ������$\frac 12$ �ĸ��ʾ������±�Ϊ <samp>10</samp>�������Ϸ������������Ϊ $8$ �֡�</p>


<pre><code class="language-input2">0011
1 0
</code></pre>



<pre><code class="language-output2">2
</code></pre>


<p>���ڷ���һ���ᷭת����Ӳ�ң����������Ժ�����Ӳ�Ҷ����泯���ˡ�</p>


<pre><code class="language-input3">0101
1 0
</code></pre>


<pre><code class="language-output3">-1
</code></pre>


<p>���ڷ��ػ�һֱ��ת��skip ��Ҳֻ��һֱ��ת���ɱ�֤��Ϸ���������</p>
<h2>������</h2>
<p>���������ء�</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1\leq n \leq 23$��$0\leq a, b \leq 998244352, 998244353\nmid a+b$��</p>
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
<td style="text-align:center;">1</td>
<td style="text-align:center;" rowspan="2">$23$</td>
<td style="text-align:center;">$a=0$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$b=0$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$a,b\leq 10$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">$23$</td>
<td style="text-align:center;">��</td>
<td style="text-align:center;">$45$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
<h2>���</h2>
<p>���� skip ��ʵ����̫���ˣ���ŭ����������� skip ��ץ��ȥ�ҳ�������</p>
