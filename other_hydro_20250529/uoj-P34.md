<p>这是一道模板题。</p>
<p>给你两个多项式，请输出乘起来后的多项式。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $n$ 和 $m$，分别表示两个多项式的次数。</p>
<p>第二行 $n + 1$ 个整数，表示第一个多项式的 $0$ 到 $n$ 次项系数。</p>
<p>第三行 $m + 1$ 个整数，表示第二个多项式的 $0$ 到 $m$ 次项系数。</p>
<h2>输出格式</h2>
<p>一行 $n + m + 1$ 个整数，表示乘起来后的多项式的 $0$ 到 $n + m$ 次项系数。</p>


<pre><code class="language-input1">1 2
1 2
1 2 1
</code></pre>


<pre><code class="language-output1">1 4 5 2
</code></pre>


<p>$(1 + 2x) \cdot (1 + 2x + x^2) = 1 + 4x + 5x^2 + 2x^3$。</p>
<h2>限制与约定</h2>
<p>$0 \leq n, m \leq 10^5$，保证输入中的系数大于等于 $0$ 且小于等于 $9$。</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20474/file/attachment.zip">样例数据下载</a></p>
