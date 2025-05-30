<p>魔法之龙玛里苟斯最近在为加基森拍卖师的削弱而感到伤心，于是他想了一道数学题。</p>
<p>$S$ 是一个可重集合，$S = \{a_1, a_2, \dots, a_n \}$。</p>
<p>等概率随机取 $S$ 的一个子集 $A = \{a_{i_1}, \dots, a_{i_m}\}$。</p>
<p>计算出 $A$ 中所有元素异或 $x$, 求 $x^k$ 的期望。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n$, $k$。</p>
<p>以下 $n$ 行每行一个整数，表示 $a_i$。</p>
<h2>输出格式</h2>
<p>如果结果是整数，直接输出。如果结果是小数（显然这个小数是有限的），输出精确值（末尾不加多余的 $0$）。</p>


<pre><code class="language-input1">4 2
0
1
2
3
</code></pre>


<pre><code class="language-output1">3.5
</code></pre>

<h2>限制与约定</h2>
<p>$1 \leq n \leq 100000$，$1 \leq k \leq 5$，$a_i \geq 0$。最终答案小于 $2^{63}$ 。$k = 1,2,3,4,5$ 各自占用 20% 的数据。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>来源</h2>
<p>中国国家队清华集训2014~2015 Day 1 - By 毕克</p>
<h2>下载</h2>
<p><a href="./20476/file/attachment.zip">样例数据下载</a></p>
