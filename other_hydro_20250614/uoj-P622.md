<p><strong>本题总用时为各测试点用时最大值。</strong></p>
<p>这是一道模板题。</p>
<p>给定一张边权非负的有向图（可能存在重边自环），请求出点 $S$ 到点 $1 \sim n$ 的最短路长度。</p>
<h2>输入格式</h2>
<p>第一行三个个正整数 $n, m, S$，表示图中点数，边数，源点编号。</p>
<p>下面 $m$ 行，每行三个整数 $u_i, v_i, w_i$，表示存在一条 $u_i$ 到达 $v_i$，边权为 $w_i$ 的边。</p>
<h2>输出格式</h2>
<p>一行 $n$ 个整数，表示 $S$ 点到每个点的最短路大小，若无法到达，则输出 <code>-1</code>。</p>


<pre><code class="language-input1">5 10 1
3 4 2
2 3 4
1 2 1
2 4 2
4 5 8
5 2 10
4 2 7
3 3 10
2 2 1
3 2 1
</code></pre>


<pre><code class="language-output1">0 1 5 3 11
</code></pre>

<h2>限制与约定</h2>
<p>对于所有数据，满足：</p>
<p>$1 \leq u_i, v_i, S \leq n$, $1 \leq n \leq 3 \times 10^5$, $1 \leq m \leq 10^6$, $0 \leq w_i \leq 10^9$。</p>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21023/file/attachment.zip">样例数据下载</a></p>
