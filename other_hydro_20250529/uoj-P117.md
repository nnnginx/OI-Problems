<p>有一天一位灵魂画师画了一张图，现在要你找出欧拉回路，即在图中找一个环使得每条边都在环上出现恰好一次。</p>
<p>一共两个子任务：</p>
<ol><li>这张图是无向图。（50分）</li>
<li>这张图是有向图。（50分）</li>
</ol><h2>输入格式</h2>
<p>第一行一个整数 $t$，表示子任务编号。$t \in \{1, 2\}$，如果 $t = 1$ 则表示处理无向图的情况，如果 $t = 2$ 则表示处理有向图的情况。</p>
<p>第二行两个整数 $n, m$，表示图的结点数和边数。</p>
<p>接下来 $m$ 行中，第 $i$ 行两个整数 $v_i, u_i$，表示第 $i$ 条边（从 $1$ 开始编号）。保证 $1 \leq v_i, u_i \leq n$。</p>
<ol><li>如果 $t = 1$ 则表示 $v_i$ 到 $u_i$ 有一条无向边。</li>
<li>如果 $t = 2$ 则表示 $v_i$ 到 $u_i$ 有一条有向边。</li>
</ol><p>图中可能有重边也可能有自环。</p>
<h2>输出格式</h2>
<p>如果不可以一笔画，输出一行 “<samp>NO</samp>”。</p>
<p>否则，输出一行 “<samp>YES</samp>”，接下来一行输出一组方案。</p>
<ol><li>如果 $t = 1$，输出 $m$ 个整数 $p_1, p_2, \dots, p_m$。令 $e = \lvert p_i \rvert$，那么 $e$ 表示经过的第 $i$ 条边的编号。如果 $p_i$ 为正数表示从 $v_e$ 走到 $u_e$，否则表示从 $u_e$ 走到 $v_e$。</li>
<li>如果 $t = 2$，输出 $m$ 个整数 $p_1, p_2, \dots, p_m$。其中 $p_i$ 表示经过的第 $i$ 条边的编号。</li>
</ol>

<pre><code class="language-input1">1
3 3
1 2
2 3
1 3
</code></pre>


<pre><code class="language-output1">YES
1 2 -3
</code></pre>



<pre><code class="language-input2">2
5 6
2 3
2 5
3 4
1 2
4 2
5 1
</code></pre>


<pre><code class="language-output2">YES
4 1 3 5 2 6
</code></pre>

<h2>限制与约定</h2>
<p>$1 \leq n \leq 10^5, 0 \leq m \leq 2 \times 10^5$</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20557/file/attachment.zip">样例数据下载</a></p>
