<p>��������Ϊ $2N$ ����������������$A,B$</p>
<p>����һ������Ϊ $2N$ ������ $C$ ��ʹ�������㣺</p>
<ul><li>���� $C$ �ĵ� $i$ ���� $C_i$ ��ֻ�ܴ� $A_i$ �� $B_i$ ��ѡȡ���� $C_i=A_i$ �� $C_i=B_i$��</li>
<li>�� $a$ Ϊ���� $A_i$ ��Ԫ�ر�ѡȡ�Ĵ�����$b$ Ϊ���� $B$ ��Ԫ�ر�ѡȡ�Ĵ������� $a=b=N$ ��ע�⵱$C_i=A_i=B_i$ʱ��������Ϊ��$A$��ѡȡ��Ҳ������Ϊ��$B$��ѡȡ</li>
<li>���� $1 \le i &lt; 2N$ ,���� $C_i \le C_{i+1}$��</li>
</ul><p>���ж�⣬�������һ��⼴�ɡ�</p>
<h2>�����ʽ</h2>
<p>��һ��һ��������$N$��</p>
<p>�ڶ���$2N$��������������$i$����������ʾ$A_i$��</p>
<p>������$2N$��������������$i$����������ʾ$B_i$��</p>
<h2>�����ʽ</h2>
<p>�������ڽ⣬���-1��</p>
<p>����һ������Ϊ$2N$�Ľ�����'A','B'���ַ���������i���ַ�Ϊ'A',��$C_i=A_i$������$C_i=B_i$��</p>


<pre><code class="language-inputundefined"><code class="sh_plain">3
2 5 4 9 15 11
6 7 6 8 12 14</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">AABABB</code>
</code></pre>

<p>����$C={2,5,6,9,12,14}$��������֤$C$��������������</p>


<pre><code class="language-inputundefined"><code class="sh_plain">2
1 4 10 20
3 5 8 13</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">BBAA</code>
</code></pre>

<p>ע�⡰AABB��Ҳ��һ��Ϸ��Ľ⡣</p>


<pre><code class="language-inputundefined"><code class="sh_plain">2
3 4 5 6
10 9 8 7</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">-1</code>
</code></pre>


<pre><code class="language-inputundefined"><code class="sh_plain">6
25 18 40 37 29 95 41 53 39 69 61 90
14 18 22 28 18 30 32 32 63 58 71 78</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">BABBABAABABA</code>
</code></pre>
<h2>���ݷ�Χ</h2>
<p>������1($11$��):$N \leq 2000$��</p>
<p>������2($89$��):$N \leq 500000$��</p>
<p>�������в������ݣ�����$1 \leq N \leq 500000,1 \leq A_i,B_i \leq 10^9$��</p>
<p>ʱ������:$\texttt{1s}$</p>
<p>�ռ�����:$\texttt{512MB}$</p>
