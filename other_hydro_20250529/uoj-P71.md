<p>����һ�������Ȩ���� $G = (V, E)$��Ȩֵ���� $w: E \rightarrow \mathbb{Z^{*}}$��������� $e$ ��Ȩֵ $w(e)$ ��Ϊ�����������͵� $s, t \in E$��ʹ���� $G' = (V, E - S)$ �ϲ����� $s$ �� $t$ ��·����</p>
<p>�� $\mathfrak{S}$ ���������������ı߼� $S$ ��ȫ������ $w(S)$  ��С������� $\mathfrak{S}$ ��ǰ $k$ С�ı߼��ı�Ȩ�͡����� $w(S) = \sum_{e \in S} w(e)$��</p>
<h2>�����ʽ</h2>
<p>��һ�а��� $5$ �������� $n, m, s, t, k$������ $s, t, k$ �������ϣ�$n, m$ �ֱ��ʾ $\lvert V \rvert, \lvert E \rvert$���������ͱ��������涨ͼ�еĽڵ��� $1$ �� $n$ ��������ʾ����֤ $s \neq t$��</p>
<p>������ $m$ �У�ÿ�� $3$ ������ $x, y, z$����ʾһ����ȨΪ $z$ �Ĵ� $x$ �� $y$ �ıߡ��������رߵ���֤û���Ի���</p>
<h2>�����ʽ</h2>
<p>��� $\lvert \mathfrak{S} \rvert &lt; k$������� $\lvert \mathfrak{S} \rvert$ �У�ÿ�а���һ����������ʾǰ $\lvert \mathfrak{S} \rvert$ �� $w(S)$�������һ��һ������ $-1$��</p>
<p>��� $\lvert \mathfrak{S} \rvert \geq k$������� $k$ �У���ʾǰ $k$ �� $w(S)$��</p>
<p>����������谴�� $w(S)$ ��С���������</p>


<pre><code class="language-input1">3 3 1 3 100
1 2 3
2 3 4
1 3 5
</code></pre>


<pre><code class="language-output1">8
9
12
-1
</code></pre>



<pre><code class="language-input2">5 8 1 5 10
1 2 45176
1 3 41088
1 4 32001
2 5 48931
3 5 39291
4 5 28970
2 3 48131
4 2 49795
</code></pre>


<pre><code class="language-output2">116468
117192
118265
120223
145438
147235
149193
157556
158280
161311
</code></pre>

<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$</th>
<th>$m$</th>
<th>$k$</th>
<th>Լ��</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$\leq 10$</td><td rowspan="2">$\leq 20$</td><td rowspan="2">$\leq 1000000$</td><td rowspan="6">��Ȩ������ $65536$</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="4">$\leq 50$</td><td rowspan="4">$\leq 100$</td><td rowspan="4">$\leq 100$</td></tr><tr><td>4</td></tr><tr><td>5</td></tr><tr><td>6</td></tr><tr><td>7</td><td rowspan="4">$\leq 3000$</td><td rowspan="8">$= 2n - 4$</td><td rowspan="4">$\leq 500000$</td><td rowspan="8">$s$ �б��������з� $t$ �ڵ㣬<br> ���з� $s$ ����б����� $t$��<br> ��Ȩ������ $2^{31} - 1$</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr><tr><td>11</td><td rowspan="4">$\leq 150000$</td><td rowspan="4">$\leq 500000$</td></tr><tr><td>12</td></tr><tr><td>13</td></tr><tr><td>14</td></tr><tr><td>15</td><td rowspan="6">$\leq 50$</td><td rowspan="6">$\leq 1500$</td><td rowspan="6">$\leq 100$</td><td rowspan="6">��Ȩ������ $65536$</td></tr><tr><td>16</td></tr><tr><td>17</td></tr><tr><td>18</td></tr><tr><td>19</td></tr><tr><td>20</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20511/file/attachment.zip">������������</a></p>
