<p><strong>存在链的测试点 $u_i = i + 1, v_i = i$ ，数据可能会更改</strong></p>
<p>欧艾大陆上有 $n$ 座城市，城市从 $1 \sim n$ 编号，所有城市经由 $n − 1$ 条无向道路互相连通，即 $n$ 座城市与 $n − 1$ 条道路构成了一棵树。</p>
<p>每座城市的集市上都会出售宝石，总共有 $m$ 种不同的宝石，用 $1 \sim m$ 编号。$i$ 号城市的集市出售的是第 $w_i$ 种宝石。一种宝石可能会在多座城市的集市出售。</p>
<p>K 神有一个宝石收集器。这个宝石收集器能按照顺序收集至多 $c$ 颗宝石，其收集宝石的顺序为:$P_1,P_2,\dots,P_c$。更具体地，收集器需要先放入第 $P_1$ 种宝石，然后才能再放入第 $P_2$ 种宝石，之后再能放入第 $P_3$ 种宝石，以此类推。其中 $P_1, P_2, \dots, P_c$ 互不相等。</p>
<p>K 神到达一个城市后，如果该城市的集市上出售的宝石种类和当前收集器中需要放入的种类相同，则他可以在该城市的集市上购买一颗宝石并放入宝石收集器中；否则他只会路过该城市什么都不做。</p>
<p>现在 K 神给了你 $q$ 次询问，每次给出起点 $s_i$ 与终点 $t_i$，他想知道如果从 $s_i$ 号城市出发，沿最短路线走到 $t_i$ 号城市后，他的收集器中最多能收集到几个宝石?（在每次询问中，收集器内初始时没有任何宝石。起点与终点城市集市上的宝石可以尝试被收集）</p>
<h2>输入格式</h2>
<p>第一行包含三个正整数 $n, m, c$，分别表示城市数，宝石种类数，收集器的容量。</p>
<p>第二行包含 $c$ 个正整数 $P_i$。数据保证 $1 \leq P_i \leq m$ 且这些数互不相等。</p>
<p>第三行包含 $n$ 个正整数 $w_i$，表示每个城市集市上出售的宝石种类。</p>
<p>接下来 $n − 1$ 行，每行两个正整数 $u_i, v_i$，表示一条连接 $u_i$ 和 $v_i$ 号城市的道路。</p>
<p>第 $n + 3$ 行包含一个正整数 $q$ 表示询问次数。</p>
<p>接下来 $q$ 行，每行两个正整数 $s_i, t_i$ 表示该次询问的起点与终点。</p>
<h2>输出格式</h2>
<p>按输入顺序输出 $q$ 行，每行一个整数表示询问的答案。</p>


<pre><code class="language-input1">7 3 3
2 3 1
2 1 3 3 2 1 3
1 2
2 3
1 4
4 5
4 6
6 7
5
3 5
1 3
7 3
5 7
7 5
</code></pre>


<pre><code class="language-output1">2
2
2
3
1
</code></pre>

<h2>样例二</h2>
<p>见附加文件中 <code>ex_gem2.in</code> 与 <code>ex_gem2.ans</code>。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_gem3.in</code> 与 <code>ex_gem3.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试数据：$1 \leq n, q \leq 2 \times 10^5, 1 \leq c \leq m \leq 5 \times 10^4, 1 \leq w_i \leq m$。</p>
<p>每个测试点的具体限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n,q \leq$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 5$</td>
<td style="text-align:center;">$1000$</td>
</tr>
<tr>
<td style="text-align:center;">$6 \sim 10$</td>
<td style="text-align:center;" rowspan="3">$2\times 10^5$</td>
<td style="text-align:center;">$m \leq 300$</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 14$</td>
<td style="text-align:center;">$u_i = i, v_i = i + 1$</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 20$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21029/file/attachment.zip">样例数据下载</a></p>
