<p>�����������죬����7����ͻȻ�����ѣ����������ˣ�����ѧ��ٵ��ˣ���</p>
<p>ʲô���첻����Ϣ����е�һ����ѣ��</p>
<p>����ѧ·�ϣ�����ܳ���һ�������ˣ���˵������������ IIIS а�̵Ŀֲ�����Ϊ���� IIIS ������� ���� ���ڰ˳�Ϊ��Ϣ�գ���ȡ�����ǵ�ʱ������ص���Ԫ321���ɱ������������Ϊ��Ϣ�յĻ�����ͽ����۹��ʵ۾�ʿ̹��һ������</p>
<p>��ʱ����°��Ѿ��Ծ��õ����˵��ϡ�</p>
<p>������˵�������������ǵ�ʱ�����������ʹ�������޷��ص���ȥ������ʷ����֪����ĺڿͼ����ܸ߳�����������ƽ�����ɣ���</p>
<p>ʱ�����������һ���� $n$ ��<strong>СдӢ����ĸ</strong>��ɵ��ַ��� $s$��</p>
<p>ʱ�����һ���ж������Ƿ���ȷ�ķ����������������˺��� $f(t)$������ $t$ ��һ���ַ�����$t_0, \dots, t_{n - 1}$ ���α�ʾ $t$ ��ÿ���ַ���</p>
<p>\begin{equation}
f(t) = \left( \sum_{k = 0}^{n-1}26^{n - k - 1} \times \mathrm{num}(t_k) \right) \bmod p
\end{equation}
���� $\mathrm{num}(c)$ ��ʾ $c$ �����ĸ����ĸ�����ŵڼ������� $0$ ��ʼ��ţ����� $\mathrm{num}(\texttt{'a'}) = 0$��$\mathrm{num}(\texttt{'g'}) = 6$����$p$ �Ǹ�<strong>����</strong>��$a \bmod b$ ��ʾ $a$ ���� $b$ ��������</p>
<p>ʱ��������������� $s$ ��ת $0, 1, \dots, {n-1}$ �εõ��ַ��� $a_0, a_1, \dots, a_{n-1}$����ν��ת���ǰ�ԭ�ַ����ĵ�һ���ַ��ŵ��ַ��������ȥ����ԭ�ַ����ڶ����ַ���Ϊ�µ��ַ����Ŀ�ʼ�����������Ҫ�����������������õ���⣩</p>
<p>ʱ����洢�� $n$ ��ֵ $h_0, h_1, \dots, h_{n - 1}$�������������һ�� $0 \leq k &lt; n$ ������ $k$ ������ $f(a_k) = h_k$����ô����������ȷ��</p>
<p>���ڸ��� $n, p$ �� $h_0, \dots, h_{n - 1}$������������롣</p>
<h2>�����ʽ</h2>
<p>��һ������������ $n, p$��������ǰ��������֤ $p &gt; 26$ ��<strong>��һ������</strong>��</p>
<p>������ $n$ �У�ÿ�а���һ���Ǹ��������α�ʾ $h_0, \dots, h_{n - 1}$����֤ $0 \leq h_0, \dots, h_{n - 1} &lt; p$��</p>
<h2>�����ʽ</h2>
<p>���һ����СдӢ����ĸ��ɵ��ַ�����ʾ��ȷ���롣</p>
<p>��֤���ٴ���һ����ȷ�����롣</p>
<p>����ж�����ȷ�����룬��ֻҪ�������һ�����ɡ�</p>


<pre><code class="language-input1">5 31
10
15
13
16
19
</code></pre>


<pre><code class="language-output1">sbvfk
</code></pre>


<p>$a_0 = \texttt{"sbvfk"}$������ת $0$ �Σ�</p>
<p>$a_1 = \texttt{"bvfks"}$������ת $1$ �Σ�</p>
<p>$a_2 = \texttt{"vfksb"}$������ת $2$ �Σ�</p>
<p>$a_3 = \texttt{"fksbv"}$������ת $3$ �Σ�</p>
<p>$a_4 = \texttt{"ksbvf"}$������ת $4$ �Σ�</p>
<p>���δ��� $f$ ��ֵ�� $10, 15, 13, 16, 19$��</p>
<p>�ٸ����ӣ�$f(\texttt{"sbvfk"}) = \left(26^4 \times 18 + 26^3 \times 1 + 26^2 \times 21 + 26^1 \times 5 + 26^0 \times 10\right) \bmod 31$</p>


<pre><code class="language-input2">4 677
0
0
0
0
</code></pre>


<pre><code class="language-output2">aaaa
</code></pre>

<h2>������Լ��</h2>
<p>�����������ݣ�$26 &lt; p \leq 10^9$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th>
<th>$n$�Ĺ�ģ</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$n \leq 5$</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="3">$n \leq 100$</td></tr><tr><td>4</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="5">$n \leq 10^5$</td></tr><tr><td>7</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20514/file/attachment.zip">������������</a></p>
