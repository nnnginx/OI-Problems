<p>B����G���ڹ��������ϡ�</p>
<p>B�������ֵ�������������������ѧ�Ѿ�������ˡ�</p>
<p>G��������ѽ��</p>
<p>B���������ϵ������ֶ������ˣ���������֮ǰ����Ҳ������������</p>
<p>G������������</p>
<p>B�����������������Ͽ����µģ���</p>
<p>G����������</p>
<p>B�������������������������~��</p>
<p>G������������</p>
<p>B���������������и�����������~��</p>
<p>G�������ʰɡ�</p>
<p>B���������� $n=3^m$ ����һ����cei ding ke��</p>
<p>G���������֣�cei ding ke ��ʲô����</p>
<p>B����������ʯͷ������~������Ҳ�ж��ִ���</p>
<p>G������������������</p>
<p>B��������Ȼᣬ�һ�û˵���ء�</p>
<h2>��������</h2>
<p>$n = 3^m$ ��������ʯͷ��������
һ���� $t$ <strong>��</strong>��Ϸ��ÿ���� $m$ <strong>��</strong>ʯͷ��������</p>
<p>��ͬһ�ֵ� $m$ ����Ϸ�У�ÿ���˵ľ��߱�������ǰȷ���ģ�Ҳ����˵���ܲ���������ԣ�Ҳ���ܸ���ǰ���ɾֵĽ��������һ�ֵľ��ߣ�
��������Ȼһ���� $n = 3^m$ �־��ߡ�</p>
<p>�� $n = 3^m$ ���˻��ȡ������ͬ�ľ��ߡ�
Ϊ�˷�������ڵ� $x$��$0 \leq x &lt; n$�����ˣ��� $x$ ת���������Ƶõ�һ��$m$λ������
���� $0$ ��ʾ������$1$ ��ʾʯͷ��$2$ ��ʾ�����͵õ��˵� $x$ ���˲�ȡ�Ĳ��ԡ�</p>
<p>���ڱ���ǹ̶��ģ����ÿ�����ڲ�ͬ�ֵ� $m$ ����Ϸ�ж����ȡͬһ�׾��ߡ�</p>
<p>�� $x$ ���������ʱ��һ������ $f_{0, x}$��</p>
<p>�ڵ� $i$ ���У���������һ���� $y$ ���� $m$ �ε�ʯͷ�������ı�����</p>
<p>������ $W \left( x, y \right)$ ��ʾ $x$ �ں� $y$ �� $m$ �α�����Ӯ�Ĵ�����
�� $L \left( x, y \right)$ ��ʾ $x$ �ں� $y$ �� $m$ �α�������Ĵ�����</p>
<p>�ڵ� $i$ �ֽ���֮�󣬵� $x$ ���˷����ǣ�</p>
<p>$$
f_{i, x} = \sum_{0 \leq y &lt; n} f_{i-1, y} b_{u, v}
$$</p>
<p>���� $u = W \left( x, y \right) = L \left( y, x \right), v = L \left( x, y \right) = W \left( y, x \right)$��ƽ�ֲ����������
$b_{u,v}$ ����һ���������������顣</p>
<p>ע�⼴ʹ $y$ �� $x$ һ�����Լ�ת�Ƶ��Լ���Ҳ�����һ��ϵ�� $b_{0, 0}$�����Լ����Լ���ȫΪƽ�֣���</p>
<p>��Ȼ��������Խ��Խ�࣬����Ҳ��Խ��Խ��
����Ʒ�ϵͳ������ƽʱ�õļ����һ����Ҳ�������
��Ҫ����ķ��� $f$ ���ڵ��� $p$ ��ʱ�򣬾ͻ��� $f \bmod p$��</p>
<p>B����֪�� $t$ ��֮�������˵ķ�����Ҳ���� $f_{t, 0}, f_{t, 1}, \ldots, f_{t, n - 1}$��</p>
<p>G�����������ҷ�������� $p$ ���������������������������������ʹ�����ǵ����ĺ͵��� $3/p$����</p>
<p>B������G���ð��������������ô���أ���</p>
<h2>�����ʽ</h2>
<p>��һ��������������ʾ $m, t, p$��</p>
<p>�ڶ����� $n = 3^m$ ����������ʾ $f_{0, 0}, f_{0, 1}, \ldots, f_{0, n - 1}$����֤ $0 \leq f_{0, i} &lt; p$��</p>
<p>�������Ĳ�����һ������ $b$���� $1$ �� $m + 1$ �������� $2$ �� $m$ ���������� $m + 1$ �� $1$ ������</p>
<p>���е� $i$ �еĵ� $j$ ����Ϊ $b_{i-1, j-1}$��$i, j \ge 1, i + j - 2 \le m$������֤ $0 \leq b_{i, j} &lt; p$��</p>
<p>������������������ʹ�����ǵ����ĺ͵��� $3/p$��
�������������� $x, y &gt; 0$��ʹ�� $1/x + 1/y = 3/p$��</p>
<h2>�����ʽ</h2>
<p>��� $n = 3^m$ �У�ÿ��һ����������ʾÿ�������յĵ÷֡�</p>
<p>���е� $i$ �б�ʾ�� $i$ ���˵ĵ÷� $f_{t, i}$��</p>


<pre><code class="language-input1">1 1 10009
10 100 1000
2 3
4
</code></pre>


<pre><code class="language-output1">4320
3240
2430
</code></pre>




<pre><code class="language-input2">2 3 103
7 8 9 10 11 12 13 14 15
1 2 3
4 5
6
</code></pre>


<pre><code class="language-output2">96
8
73
38
53
15
27
42
4
</code></pre>


<h2>������Լ��</h2>
<p>�����������ݣ�$0 \leq m \leq 12$��$0 \leq t \leq 10^{9}$��$1 \leq p \leq 10^{9}$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե�</th><th rowspan="1">$m$</th><th rowspan="1">$t$</th><th rowspan="1">$p$</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">$= 3$</td><td rowspan="2">$\leq 10^{3}$</td><td rowspan="8">����������</td></tr><tr><td rowspan="1">2</td><td rowspan="1">$= 4$</td></tr><tr><td rowspan="1">3</td><td rowspan="1">$= 3$</td><td rowspan="18">$\leq 10^{9}$</td></tr><tr><td rowspan="1">4</td><td rowspan="1">$= 4$</td></tr><tr><td rowspan="1">5</td><td rowspan="1">$= 5$</td></tr><tr><td rowspan="1">6</td><td rowspan="1">$= 5$</td></tr><tr><td rowspan="1">7</td><td rowspan="1">$= 6$</td></tr><tr><td rowspan="1">8</td><td rowspan="1">$= 7$</td></tr><tr><td rowspan="1">9</td><td rowspan="1">$= 9$</td><td rowspan="4">$\leq 7$</td></tr><tr><td rowspan="1">10</td><td rowspan="1">$= 10$</td></tr><tr><td rowspan="1">11</td><td rowspan="1">$= 11$</td></tr><tr><td rowspan="1">12</td><td rowspan="1">$= 12$</td></tr><tr><td rowspan="1">13</td><td rowspan="1">$= 9$</td><td rowspan="4">������</td></tr><tr><td rowspan="1">14</td><td rowspan="1">$= 10$</td></tr><tr><td rowspan="1">15</td><td rowspan="1">$= 11$</td></tr><tr><td rowspan="1">16</td><td rowspan="1">$= 12$</td></tr><tr><td rowspan="1">17</td><td rowspan="1">$= 9$</td><td rowspan="4">����������</td></tr><tr><td rowspan="1">18</td><td rowspan="1">$= 10$</td></tr><tr><td rowspan="1">19</td><td rowspan="1">$= 11$</td></tr><tr><td rowspan="1">20</td><td rowspan="1">$= 12$</td></tr></tbody></table></div>


<p><strong>ʱ������</strong>��$2\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20701/file/attachment.zip">������������</a></p>
