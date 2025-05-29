<p>组合数 $C_n^m$ 表示的是从 $n$ 个物品中选出 $m$ 个物品的方案数。举个例子，从 $(1,2,3)$ 三个物品中选择两个物品可以有 $(1,2),(1,3),(2,3)$ 这三种选择方法。根据组合数的定义，我们可以给出计算组合数 $C_n^m$ 的一般公式：</p>
<p>$$C_n^m=\frac{n!}{m!(n-m)!}$$</p>
<p>其中 $n!=1\times2\times\cdots\times n$。（额外的，当 $n=0$ 时， $n!=1$）</p>
<p>小葱想知道如果给定 $n,m$ 和 $k$，对于所有的 $0\leq i\leq n,0\leq j\leq \min \left ( i, m \right )$ 有多少对 $(i,j)$ 满足 $C_i^j$ 是 $k$ 的倍数。</p>
<p>答案对 $10^9 + 7$ 取模。</p>
<h2>输入格式</h2>
<p>第一行有两个整数 $t,k$，其中 $t$ 代表该测试点总共有多少组测试数据。</p>
<p>接下来 $t$ 行每行两个整数 $n,m$。</p>
<h2>输出格式</h2>
<p>$t$ 行，每行一个整数代表所有的 $0\leq i\leq n,0\leq j\leq \min \left ( i, m \right )$ 中有多少对 $(i,j)$ 满足 $C_i^j$ 是 $k$ 的倍数。</p>


<pre><code class="language-input1">1 2
3 3
</code></pre>


<pre><code class="language-output1">1
</code></pre>


<p>在所有可能的情况中，只有 $C_2^1=2$ 是 $2$ 的倍数。</p>


<pre><code class="language-input2">2 5
4 5
6 7
</code></pre>


<pre><code class="language-output2">0
7
</code></pre>



<pre><code class="language-input3">3 23
23333333 23333333
233333333 233333333
2333333333 2333333333
</code></pre>


<pre><code class="language-output3">851883128
959557926
680723120
</code></pre>


<h2>限制与约定</h2>
<p>对于 $20\%$ 的测试点，$1\leq n,m\leq 100$；</p>
<p>对于另外 $15\%$ 的测试点，$n\leq m$；</p>
<p>对于另外 $15\%$ 的测试点， $k=2$；</p>
<p>对于另外 $15\%$ 的测试点， $m\leq 10$；</p>
<p>对于 $100\%$ 的测试点， $1\leq n,m\leq 10^{18},1 \leq t,k\leq 100$，且 $k$ 是一个质数。</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20704/file/attachment.zip">样例数据下载</a></p>
