<p>����һ�� $n$ ���� $m$ ���߹��ɵ�����ͼ $G=(V, E)$�����е�� $1$ �� $n$ ��ţ��� $i$ ���ߵ����Ϊ $from(i)$���յ�Ϊ $to(i)$�������� $cap(i)$ �ͷ��� $cost(i)$ �������ԡ����ң�ͼ�д�����������㣬Դ�� $s$ �ͻ�� $t$��$s$ ��û����ߣ�$t$ ��û�г��ߡ�</p>
<p>���������� $f:E\rightarrow N$ Ϊ����������������һ�������� $f(i)$ ��ʾ $i$ �����ߵ���������</p>
<ol>
<li><p>$\forall i\in E, 0\le f(i)\le cap(i)$��ÿ���ߵ�������������������</p>
</li>
<li><p>$\forall u\in (V\setminus\{s, t\}), \sum\limits_{from(i) = u\ }f(i)=\sum\limits_{to(i) = u\ }f(i)$����Դ����ÿ�������������������������</p>
</li>
</ol>
<p>����һ��������������Ϊ $s$ ������������$flow(f)=\sum_{from(i)=s\ \ \,}f(i)$��</p>
<p>����һ�����������ܷ���Ϊÿ���ߵ���������ó˻�֮�ͣ�$totalcost(f)=\sum_{i\in E\;}f(i) \cdot cost(i)$��</p>
<p>������������$flow(f)$ �����ֵ�����Լ������ǰ���µ���С���ã��� $\min\{totalcost(f)|flow(f)=\max\{flow(i)|i\text{ is a flow of }G\}\}$����</p>
<h2>�����ʽ</h2>
<p>����ĵ�һ�а����ĸ������� $n$, $m$, $s$, $t$���ֱ��ʾͼ�ĵ����ͱ�����Դ��ͻ�㡣</p>
<p>������ $m$ ���еĵ� $i$ �а����ĸ����� $from(i)$, $to(i)$, $cap(i)$, $cost(i)$���ֱ��ʾͼ�е� $i$ ���ߵ���㣬�յ㣬���������á�</p>
<h2>�����ʽ</h2>
<p>������������������ֱ��ʾ������������ǰ���µ���С���á�</p>


<pre><code class="language-input1"><code class="sh_plain">4 5 4 3
4 2 30 2
4 3 20 3
2 3 20 1
2 1 30 9
1 3 40 5</code>
</code></pre>

<pre><code class="language-output1"><code class="sh_plain">50 280</code>
</code></pre>

<p>�� $f(u, v)$ ��ָ $u$ �� $v$ �����ߵ���������ôȡ�������ǰ���µ���С����ʱ��$f(4, 2)=30$, $f(4, 3)=20$, $f(2, 3)=20$, $f(2, 1)=10$, $f(1, 3)=10$ ��</p>


<pre><code class="language-input2"><code class="sh_plain">3 1 1 3
2 2 1 -1</code>
</code></pre>

<pre><code class="language-output2"><code class="sh_plain">0 -1</code>
</code></pre>

<p>һ���Ϸ�����ֻ��������������������ƽ�⣬һ���� $s$, $t$ ����ͨ�Ļ�Ҳ��������������������������ֲ���ͨ����������õĻ���<a href="https://codeforces.com/blog/entry/57018?#comment-406791">���Թ�Լ�����ܶٻ�·����</a>����</p>
<h2>������Լ��</h2>
<p>���� $100\%$ �����ݣ�$1\le n, m\le 500$��$1\le s, t\le n$��$s\ne t$��$1\le from(i), to(i)\le n$��$from(i)\ne t$��$to(i)\ne s$��$1\le cap(i)\le 10^9$��$-2\cdot 10^6\le cost(i)\le 2\cdot 10^6$��</p>
<p><strong>ʱ�����ƣ�</strong>$5\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>��ʾ</h2>
<p>�����������㷨�ĸ��Ӷ�Ϊ $O(nmf)$ (���� $f$ ��ʾ������Ĵ�С)�������޷�ͨ�����⡣</p>
<p>һ�ֿ��еĽ��������ʹ�� <a href="https://ouuan.github.io/post/%E5%9F%BA%E4%BA%8E-capacity-scaling-%E7%9A%84%E5%BC%B1%E5%A4%9A%E9%A1%B9%E5%BC%8F%E5%A4%8D%E6%9D%82%E5%BA%A6%E6%9C%80%E5%B0%8F%E8%B4%B9%E7%94%A8%E6%B5%81%E7%AE%97%E6%B3%95/">���� Capacity Scaling ��������ʽ���Ӷ���С�������㷨</a> ��</p>
