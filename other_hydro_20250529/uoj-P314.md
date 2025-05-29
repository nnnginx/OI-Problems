<p>P ��ʿ�����ļ����������Ϊ��һ�������Ĳ�����</p>
<p>������˵����һ������ $x$ ��һ��ʼΪ0��</p>
<p>�������� $n$ ��������ÿ�����������������������е�һ�֣�</p>
<ul><li><code>1</code> $a$ $b$ ���� $x$ �������� $a \cdot 2 ^ b$������ $a$ Ϊһ��������$b$ Ϊһ���Ǹ�����</li>
<li><code>2</code> $k$ ��ѯ�� $x$ ���ö����Ʊ�ʾʱ��λȨΪ $2 ^ k$ ��λ��ֵ������һλ�ϵ� $1$ ���� $2 ^ k$ ��</li>
</ul><p>��֤���κ�ʱ��$x \ge 0$��</p>
<h2>�����ʽ</h2>
<p>�ӱ�׼����������ݡ�</p>
<p>����ĵ�һ�а����ĸ������� $n, t_1, t_2, t_3$��$n$ �ĺ������Ŀ������$t_1, t_2, t_3$ �ľ��庬���������</p>
<p>������ $n$ �У�ÿ�и���һ�������������ʽ�ͺ������Ŀ������</p>
<p>ͬһ���������������Ԫ��֮�䣬��ǡ��һ���ո������</p>
<h2>�����ʽ</h2>
<p>�������׼�����</p>
<p>����ÿ��ѯ�ʲ��������һ�У���ʾ��ѯ�ʵĴ𰸣�0��1����
���ڼӷ�������û���κ������</p>


<pre><code class="language-input1">10 3 1 2
1 100 0
1 2333 0
1 -233 0
2 5
2 7
2 15
1 5 15
2 15
1 -1 12
2 15
</code></pre>




<pre><code class="language-output1">0
1
0
1
0
</code></pre>



<p>�������� $10$ ��������
�� $1$ ��Ϊ�� $x$ ���� $100 \times 2^0$ �������� $x= 100$ ��</p>
<p>�� $2$ ��Ϊ�� $x$ ���� $2333 \times 2^0$ �������� $x= 2433$ ��</p>
<p>�� $3$ ��Ϊ�� $x$ ���� $-233 \times 2^0$ �������� $x= 2200$ ��</p>
<p>�� $4$ ��Ϊѯ�� $x$ λȨΪ $2^5$ ��λ�ϵ�ֵ�� $x$ �ڶ�������Ϊ $100010011000$ ����Ϊ $0$ ��</p>
<p>�� $5$ ��Ϊѯ�� $x$ λȨΪ $2^7$ ��λ�ϵ�ֵ�� $x$ �ڶ�������Ϊ $100010011000$ ����Ϊ $1$ ��</p>
<p>�� $6$ ��Ϊѯ�� $x$ λȨΪ $2^{15}$ ��λ�ϵ�ֵ�� $x$ �ڶ�������Ϊ $100010011000$ ����Ϊ $0$ ��</p>
<p>�� $7$ ��Ϊ�� $x$ ���� $5 \times 2^{15} = 163840$ �������� $x= 166040$ ��</p>
<p>�� $8$ ��Ϊѯ�� $x$ λȨΪ $2^{15}$ ��λ�ϵ�ֵ�� $x$ �ڶ�������Ϊ $101000100010011000$ ����Ϊ $1$ ��</p>
<p>�� $9$ ��Ϊ�� $x$ ���� $-1 \times 2^{12} = -4096$ �������� $x= 161944$ ��</p>
<p>�� $10$ ��Ϊѯ�� $x$ λȨΪ $2^{15}$ ��λ�ϵ�ֵ�� $x$ �ڶ�������Ϊ $100111100010011000$ ����Ϊ $0$ ��</p>
<h2>������</h2>
<p>�������ļ��е� <em>ex_integer2.in</em> �� <em>ex_integer2.ans</em>��</p>
<p>�������������ݷ�Χͬ��7�����Ե㡣</p>
<h2>������</h2>
<p>�������ļ��е� <em>ex_integer3.in</em> �� <em>ex_integer3.ans</em>��</p>
<p>�������������ݷ�Χͬ��13�����Ե㡣</p>
<h2>������</h2>
<p>�������ļ��е� <em>ex_integer4.in</em> �� <em>ex_integer4.ans</em>��</p>
<p>�������������ݷ�Χͬ��14�����Ե㡣</p>
<h2>������Լ��</h2>
<p>�����в��Ե��У�$1 \le t_1 \le 3, 1 \le t_2 \le 4, 1 \le t_3 \le 2$��
��ͬ�� $t_1, t_2, t_3$ ��Ӧ�������������£�</p>
<ul><li>���� $t_1 = 1$ �Ĳ��Ե㣬���� $a = 1$</li>
<li>���� $t_1 = 2$ �Ĳ��Ե㣬���� $|a| = 1$</li>
<li>���� $t_1 = 3$ �Ĳ��Ե㣬���� $|a| \le 10 ^ 9$</li>
<li>���� $t_2 = 1$ �Ĳ��Ե㣬���� $0 \le b,k \le 30$</li>
<li>���� $t_2 = 2$ �Ĳ��Ե㣬���� $0 \le b,k \le 100$</li>
<li>���� $t_2 = 3$ �Ĳ��Ե㣬���� $0 \le b,k \le n$</li>
<li>���� $t_2 = 4$ �Ĳ��Ե㣬���� $0 \le b,k \le 30 n$</li>
<li>���� $t_3 = 1$ �Ĳ��Ե㣬��֤����ѯ�ʲ������������޸Ĳ���֮��</li>
<li>���� $t_3 = 2$ �Ĳ��Ե㣬����֤ѯ�ʲ������޸Ĳ������Ⱥ�˳��</li>
</ul><p>���⹲25�����Ե㣬ÿ�����Ե�4�֡��������Ե�����ݷ�Χ���£�</p>
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th><th rowspan="1">$n \le$</th><th rowspan="1">$t_1$</th><th rowspan="1">$t_2$</th><th rowspan="1">$t_3$</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">$10$</td><td rowspan="3">3</td><td rowspan="1">1</td><td rowspan="4">2</td></tr><tr><td rowspan="1">2</td><td rowspan="1">$100$</td><td rowspan="2">2</td></tr><tr><td rowspan="1">3</td><td rowspan="1">$2000$</td></tr><tr><td rowspan="1">4</td><td rowspan="1">$4000$</td><td rowspan="1">1</td><td rowspan="3">3</td></tr><tr><td rowspan="1">5</td><td rowspan="1">$6000$</td><td rowspan="1">3</td><td rowspan="1">1</td></tr><tr><td rowspan="1">6</td><td rowspan="1">$8000$</td><td rowspan="1">2</td><td rowspan="4">2</td></tr><tr><td rowspan="1">7</td><td rowspan="1">$9000$</td><td rowspan="5">3</td><td rowspan="1">4</td></tr><tr><td rowspan="1">8</td><td rowspan="1">$10000$</td><td rowspan="1">3</td></tr><tr><td rowspan="1">9</td><td rowspan="1">$30000$</td><td rowspan="2">4</td></tr><tr><td rowspan="1">10</td><td rowspan="1">$50000$</td><td rowspan="1">1</td></tr><tr><td rowspan="1">11</td><td rowspan="1">$60000$</td><td rowspan="1">3</td><td rowspan="12">2</td></tr><tr><td rowspan="1">12</td><td rowspan="1">$65000$</td><td rowspan="1">2</td><td rowspan="5">4</td></tr><tr><td rowspan="1">13</td><td rowspan="1">$70000$</td><td rowspan="2">3</td></tr><tr><td rowspan="1">14</td><td rowspan="1">$200000$</td></tr><tr><td rowspan="1">15</td><td rowspan="1">$300000$</td><td rowspan="1">2</td></tr><tr><td rowspan="1">16</td><td rowspan="1">$400000$</td><td rowspan="4">3</td></tr><tr><td rowspan="1">17</td><td rowspan="1">$500000$</td><td rowspan="1">3</td></tr><tr><td rowspan="1">18</td><td rowspan="1">$600000$</td><td rowspan="4">4</td></tr><tr><td rowspan="1">19</td><td rowspan="1">$700000$</td></tr><tr><td rowspan="1">20</td><td rowspan="1">$800000$</td><td rowspan="1">1</td></tr><tr><td rowspan="1">21</td><td rowspan="1">$900000$</td><td rowspan="1">2</td></tr><tr><td rowspan="1">22</td><td rowspan="1">$930000$</td><td rowspan="4">3</td><td rowspan="1">3</td></tr><tr><td rowspan="1">23</td><td rowspan="1">$960000$</td><td rowspan="1">4</td><td rowspan="1">1</td></tr><tr><td rowspan="1">24</td><td rowspan="1">$990000$</td><td rowspan="1">3</td><td rowspan="2">2</td></tr><tr><td rowspan="1">25</td><td rowspan="1">$1000000$</td><td rowspan="1">4</td></tr></tbody></table><p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20741/file/attachment.zip">������������</a></p>
