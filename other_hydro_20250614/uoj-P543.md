<p>����һ�� $n$ �������и��� $T$������ $1$ ��ʼ��ţ������Ϊ $1$ �Ž�㣬ÿ�������һ��������Ȩֵ $v_i$��</p>
<p>�� $x$ �Ž��������ڣ����� $x$ ���������н����Ϊ $c_1, c_2, \dots, c_k$������ $x$ �ļ�ֵΪ��</p>
<p>$$
val(x) = (v_{c_1} + d(c_1, x)) \oplus (v_{c_2} + d(c_2, x)) \oplus \cdots \oplus (v_{c_k} + d(c_k, x))
$$</p>
<p>���� $d(x, y)$ ��ʾ���� $x$ �Ž���� $y$ �Ž���Ψһ��·���������ı�����$d(x, x) = 0$��$\oplus$ ��ʾ������㡣</p>
<p>������� $\sum_{i=1}^n val(i)$ �Ľ����</p>
<h2>�����ʽ</h2>
<p>��һ��һ�������� $n$ ��ʾ���Ĵ�С��</p>
<p>�ڶ��� $n$ ����������ʾ $v_i$��</p>
<p>������һ�� $n-1$ �������������α�ʾ $2$ �Ž�㵽 $n$ �Ž�㣬ÿ�����ĸ��ױ�� $p_i$��</p>
<h2>�����ʽ</h2>
<p>һ��һ��������ʾ�𰸡�</p>


<pre><code class="language-inputundefined"><code class="sh_plain">5
5 4 1 2 3
1 1 2 2</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">12</code>
</code></pre>

<p>$val(1) = (5 + 0)\oplus(4 + 1)\oplus(1 + 1)\oplus(2 + 2)\oplus(3 + 2) = 3$��</p>
<p>$val(2) = (4 + 0)\oplus(2 + 1)\oplus(3 + 1) = 3$��</p>
<p>$val(3) = (1 + 0) = 1$��</p>
<p>$val(4) = (2 + 0) = 2$��</p>
<p>$val(5) = (3 + 0) = 3$��</p>
<p>��Ϊ $12$��</p>
<h2>����2</h2>
<p>�������ļ��� <code>ex_tree2.in</code> �� <code>ex_tree2.ans</code>��</p>
<h2>���ݷ�Χ</h2>
<p>����ǰ $10\%$ �����ݣ�$1\le n\le 2501$��</p>
<p>����ǰ $40\%$ �����ݣ�$1\le n\le 152501$��</p>
<p>���� $20\%$ �����ݣ����� $p_i = i - 1 (2\le i\le n)$��</p>
<p>���� $20\%$ �����ݣ����� $v_i = 1 (1\le i\le n)$��</p>
<p>���� $100\%$ �����ݣ�$1\le n, v_i \le 525010, 1\le p_i\le n$��</p>
<p><strong>ʱ������:</strong> $2\texttt{s}$</p>
<p><strong>�ռ�����:</strong> $512\texttt{MB}$</p>
<p><a href="http://uoj.ac/download.php?type=problem&amp;id=543">�����ļ�</a></p>
