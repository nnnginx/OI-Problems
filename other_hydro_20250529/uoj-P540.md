<p>������֪��С��ͬѧ�ó����㣬�����ó������������С������ϣ�������</p>
<p>$$
\left(\sum_{k=0}^n f(k) \times x^k \times \binom n k\right) \bmod p
$$</p>
<p>��ֵ������ $n, x, p$ Ϊ������������$f(k)$ Ϊ������һ�� $m$ �ζ���ʽ $f(k) = a_0 + a_1 k + a_2 k^2 + \cdots + a_m k^m$��</p>
<p>$\binom n k$ Ϊ���������ֵΪ $\binom n k = \frac{n!}{k!(n-k)!}$��</p>
<h2>�����ʽ</h2>
<p>��һ���ĸ��Ǹ����� $n, x, p, m$��</p>
<p>�ڶ��� $m + 1$ ���������ֱ���� $a_0, a_1, \cdots, a_m$��</p>
<h2>�����ʽ</h2>
<p>һ��һ��������ʾ�𰸡�</p>


<pre><code class="language-inputundefined"><code class="sh_plain">5 1 10007 2
0 0 1</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">240</code>
</code></pre>

<p>$f(0) = 0��f(1) = 1��f(2) = 4��f(3) = 9��f(4) = 16��f(5) = 25$��</p>
<p>$x = 1$���� $x^k$ ��Ϊ $1$���˻��еĸ�����Ժ��ԡ�</p>
<p>$\binom 5 0 = 1, \binom 5 1 = 5, \binom 5 2 = 10, \binom 5 3 = 10, \binom 5 4 = 5, \binom 5 5 = 1$��</p>
<p>���մ�Ϊ��</p>
<p>$$
\sum_{k=0}^5 f(5) \times \binom 5 k = 0\times 1 + 1\times 5 + 4\times 10 + 9\times 10 + 16\times 5 + 25\times 1 = 240
$$</p>


<pre><code class="language-inputundefined"><code class="sh_plain">996 233 998244353 5
5 4 13 16 20 15</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">869469289</code>
</code></pre>
<h2>����3</h2>
<p>�������ļ��� <code>ex_problem3.in</code> �� <code>ex_problem3.ans</code>��</p>
<h2>���ݷ�Χ</h2>
<p>�������в������ݣ�$1\le n, x, p \le 10^9, 0\le a_i\le 10^9, 0\le m \le \min(n,1000)$��</p>
<p>ÿ�����Ե�ľ������Ƽ��±�</p>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle">
        <thead><tr><th>���Ե���</th><th>$n \le$</th><th>$m \le$</th><th>������������</th></tr></thead>
        <tbody>
               <tr><td>$1 \sim 3$</td><td>$1000$</td><td>$1000$</td><td>��</td></tr>
               <tr><td>$4 \sim 6$</td><td>$10^5$</td><td rowspan="2">$0$</td><td>$p$������</td></tr>
               <tr><td>$7 \sim 8$</td><td rowspan="4">$10^9$</td><td rowspan="2">��</td></tr>
               <tr><td>$9 \sim 12$</td><td>$5$</td></tr>
               <tr><td>$13 \sim 16$</td><td rowspan="2">$1000$</td><td>$x=1$</td></tr>
               <tr><td>$17 \sim 20$</td><td>��</td></tr>
        </tbody>
    </table>
</div>

<p><strong>ʱ������:</strong> $1\texttt{s}$</p>
<p><strong>�ռ�����:</strong> $512\texttt{MB}$</p>
<p><a href="http://uoj.ac/download.php?type=problem&amp;id=540">������������</a></p>
