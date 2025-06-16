<p>��ѧ���ԣ�һ��Բ׶���ߵ�����ס���㣬�㿪ʼ���ر��㡣���ǣ�����ʵ��̫�ѣ����������ÿ��˼·�ೢ�Գ��ԡ�</p>
<p>���˼ά���̿���ת��Ϊ���¹��̣�</p>
<ul><li>��һ����������������и��ڲ����� $x$ ��ʼʱΪ $x_0$��ÿ�β��������ʱ���Ὣ $x$ ��Ϊ $(100000005x+20150609) \bmod 998244353$��Ȼ�󷵻� $\lfloor \frac{x}{100} \rfloor$����$a \bmod b$ ��ʾ $a$ ���� $b$ ������������������ȼ����ڼӼ�����$\lfloor \alpha \rfloor$ ��ʾ $\alpha$ ����ȡ����Ľ������</li>
<li>��ʼʱ�� $n$ ���㣬�ֱ���Ϊ $1, \dots, n$������Ŵ�С����˳�����ɵ� $i$ ��������꣺<ul><li>�Ѻ����긳Ϊ $i$��</li>
<li>����һ������� $\hat{y}$���������긳Ϊ $\hat{y} \bmod 100001$��</li>
</ul></li>
<li>�� $m$ ����������ʾ���˼·���̡������������֣�<ul><li><samp>C</samp>����˳���������� $\hat{p}, \hat{y}$���� $p = \hat{p} \bmod n + 1, y = \hat{y} \bmod 100001$��Ȼ��ѵ� $p$ ������������޸�Ϊ $y$��</li>
<li><samp>R</samp>����˳���������� $\hat{p}, \hat{q}$���� $p = \min\{\hat{p} \bmod n + 1, \hat{q} \bmod n + 1\}, q = \max\{\hat{p} \bmod n + 1, \hat{q} \bmod n + 1\}$���ѱ�Ŵ��ڵ��� $p$ С�ڵ��� $q$ �ĵ�������� $y$ ��Ϊ $100000 - y$��</li>
<li><samp>Q $a$ $b$ $c$</samp>����ѯ��������˳���������� $\hat{p}, \hat{q}$���� $p = \min\{\hat{p} \bmod n + 1, \hat{q} \bmod n + 1\}, q = \max\{\hat{p} \bmod n + 1, \hat{q} \bmod n + 1\}$������С������ $t$ ʹ�ã��������б�Ŵ��ڵ��� $p$ С�ڵ��� $q$ �ĵ� $(x, y)$ ������ $ax + by + cxy \leq t$����$a, b, c$ ��Ϊ�Ǹ�������</li>
</ul></li>
</ul><h2>�����ʽ</h2>
<p>��һ���������� $n, m, x_0$����֤ $n, m \geq 1$��$0 \leq x_0 &lt; 998244353$ �� $x_0 \neq 340787122$��</p>
<p>������ $m$ �У�ÿ�б�ʾһ����������ʽ��ǰ������</p>
<h2>�����ʽ</h2>
<p>����ÿ����ѯ�������һ��������ʾ��С�� $t$��</p>


<pre><code class="language-input1">3 3 2705443
C
R
Q 872784 195599 7
</code></pre>


<pre><code class="language-output1">13035048532
</code></pre>


<p>�ʼ�����������ֱ��� $(1,91263),(2,33372),(3,10601)$��</p>
<p>��һ�������ѵ������������ĳ��� $(3,94317)$��</p>
<p>�ڶ��������޸������� $[2,3]$���ڶ��������� $(2,66628)$�������������� $(3,5683)$��</p>
<p>���һ������ѯ������ $[2,3]$�����Է�����С�� $t$ �� $13035048532$��</p>
<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<p>���������У��������в�ѯ������֤ $0 \leq a, b &lt; 10^6$��$0 \leq c &lt; 40$��<strong>��֤��ѯ�����ĳ��ִ��������� $10^5$</strong>��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$�Ĺ�ģ</th>
<th>$m$�Ĺ�ģ</th>
<th>��������</th>
</tr></thead><tbody><tr><td>1</td><td>$n \leq 100$</td><td>$m \leq 100$</td><td>��</td></tr><tr><td>2</td><td rowspan="2">$n \leq 10^5$</td><td rowspan="2">$m \leq 10^6$</td><td rowspan="2">���в�ѯ������ $a = c = 0$</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="2">$n \leq 10^5$</td><td rowspan="2">$m \leq 2 \times 10^5$</td><td rowspan="2">���в�ѯ������ $c = 0$</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="2">$n \leq 10^5$</td><td rowspan="2">$m \leq 2 \times 10^5$</td><td rowspan="2">��</td></tr><tr><td>7</td></tr><tr><td>8</td><td rowspan="3">$n \leq 10^5$</td><td rowspan="3">$m \leq 10^6$</td><td rowspan="3">��</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20559/file/attachment.zip">������������</a></p>
