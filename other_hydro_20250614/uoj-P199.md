<p>С P ������ NOIP2044 �������ϣ������ֵڶ������Ŀ�������ģ�����һ������Ϊ $n$ ���ַ��������ַ��������� $m$ �ֲ�ͬ���ַ���ɣ����е� $i$ ���ַ��ĳ��ִ��������� $c_i$����������ַ����ĺ�׺������ʲô��</p>
<p>������С P �뵽��һ���µ�����ϣ��������æ�������Ŀ�����������£����ж����ֲ�ͬ�Ĵ𰸡�Ҳ���������� $m$ ���ַ���ɣ����е� $i$ ���ַ����ִ��������� $c_i$���ҳ���Ϊ $n$ ���ַ��������ж����ֲ�ͬ�ĺ�׺���顣</p>
<p>���ڴ𰸺ܴ���ֻ������𰸶� $10^9+7$ ȡģ�������</p>
<p>����һ���ַ��� $s=s_1s_2...s_n$���� $\mathrm{suf}(i)$ ��ʾ $i$ ���λ�õ�ĩβ���Ӵ�����׺����Ϊһ�� $1$ �� $n$ ������ $p_1,p_2,...,p_n$������ $\mathrm{suf}(p_1)&lt; \mathrm{suf}(p_2)&lt; \dots &lt; \mathrm{suf}(p_n)$�����������ַ��� $s$ �� $t$���� $i$ Ϊ��һ��ʹ�� $s_i \neq t_i$ ��λ�ã���ô���� $s_i$ �� $t_i$ ��С�Ķ�Ӧ���ַ�����С����� $i$ �����ڣ���ô����С���ַ�����С��</p>
<p>�����ַ���֮��Ĵ�С��ϵ�����ǹ涨�� $1$ ���ַ���С���� $2$ ���ַ���С���Դ����ơ�</p>
<h2>�����ʽ</h2>
<p>����ĵ�һ�а������������� $n,m$����ʾ�ַ����ĳ���Ϊ $n$������ $m$ ���ַ���</p>
<p>������һ�У����� $m$ ���Ǹ����� $c_1,c_2,...,c_m$����ʾÿ���ַ����ĳ��ִ�������֤ $0 \leq c_1,c_2,...,c_m \leq n,c_1+c_2+...+c_m \geq n$��</p>
<h2>�����ʽ</h2>
<p>�����һ�У�����һ����������ʾ�𰸡�</p>


<pre><code class="language-input1">3 2
2 2
</code></pre>


<pre><code class="language-output1">5
</code></pre>


<p>���Ǽ� $a$ Ϊ��һ���ַ���$b$ Ϊ�ڶ����ַ�����ô���� $aab,aba,abb,baa,bab,bba$ �����ֿ��ܵ��ַ��������ǵĺ�׺����Ϊ
\begin{equation}
(1,2,3),(3,1,2),(1,3,2),(3,2,1),(2,3,1),(3,2,1).
\end{equation}
���Թ��� $5$ �ֲ�ͬ�Ľ����</p>


<pre><code class="language-input2">10 5
2 3 4 3 2
</code></pre>


<pre><code class="language-output2">1003811
</code></pre>

<h2>������</h2>
<p>��������������</p>
<h2>������Լ��</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>$n$</th><th>$m$</th><th>Լ��</th></tr></thead><tbody><tr><td>1</td><td>$\leq 6$</td><td>$\leq 6$</td><td rowspan="4">��</td></tr><tr><td>2-3</td><td>$\leq 10$</td><td>$\leq 10$</td></tr><tr><td>4</td><td rowspan="3">$\leq 500$</td><td>$=2$</td></tr><tr><td>5</td><td>$=3$</td></tr><tr><td>6-7</td><td>$\leq 500$</td><td>$c_1=c_2=...=c_m=n$</td></tr><tr><td>8-10</td><td>$\leq 50$</td><td>$\leq 50$</td><td rowspan="3">��</td></tr><tr><td>11-14</td><td>$\leq 200$</td><td>$\leq 200$</td></tr><tr><td>15-20</td><td>$\leq 500$</td><td>$\leq 500$</td></tr></tbody></table></div>

<p><strong>ʱ�����ƣ�</strong>$5\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20639/file/attachment.zip">������������</a></p>
