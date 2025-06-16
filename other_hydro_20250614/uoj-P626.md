<p>对于一张 $n$ 个点 $m$ 条边的有向图 $G$ (顶点从 $1 \sim n$ 编号)，定义函数 $f(u, G)$ :</p>
<ol>
<li>初始化返回值 $cnt = 0$，图 $G′ = G$。</li>
<li>从 $1$ 至 $n$ 按顺序枚举顶点 $v$，如果当前的图 $G′$ 中，从 $u$ 到 $v$ 与从 $v$ 到 $u$ 的路径都存在，则将 $cnt + 1$，并在图 $G′$ 中删去顶点 $v$ 以及与它相关的边。</li>
<li>第 $2$ 步结束后，返回值 $cnt$ 即为函数值。</li>
</ol>
<p>现在给定一张有向图 G,请你求出 $h(G) = f(1, G) + f(2, G) + \dots + f(n, G)$ 的值。</p>
<p>更进一步地，记删除（按输入顺序给出的）第 $1 \sim i$ 条边后的图为 $G_i (1 \leq i \leq m)$，请你求出所有 $h(G_i)$ 的值。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $n, m$ 表示图的点数与边数。</p>
<p>接下来 $m$ 行每行两个整数，第 $i$ 行的两个整数 $x_i, y_i$ 表示一条有向边 $x_i \rightarrow y_i$。</p>
<p>数据保证 $x_i \neq y_i$ 且同一条边不会给出多次。</p>
<h2>输出格式</h2>
<p>输出一行 $m + 1$ 个整数，其中第一个数表示给出的完整图 $G$ 的 $h(G)$ 值。第 $i (2 \leq i \leq m + 1)$ 个整数表示 $h(G_{i-1})$。</p>


<pre><code class="language-input1">4 6
2 3
3 2
4 1
1 4
2 1
3 1
</code></pre>


<pre><code class="language-output1">6 5 5 4 4 4 4
</code></pre>


<p>对于给出的完整图 $G$:</p>
<ol>
<li>$f (1, G) = 1$，过程中删除了顶点 $1$。</li>
<li>$f (2, G) = 1$，过程中删除了顶点 $2$。</li>
<li>$f (3, G) = 2$，过程中删除了顶点 $2, 3$。</li>
<li>$f (4, G) = 2$，过程中删除了顶点 $1, 4$。</li>
</ol>
<h2>样例二</h2>
<p>见附加文件中 <code>ex_graph2.in</code> 与 <code>ex_graph2.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试数据：$2 \leq n \leq 1000, 1 \leq m \leq 2 \times 10^5, 1 \leq x_i, y_i \leq n$。</p>
<p>每个测试点的具体限制见下表:</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \leq$</th>
<th style="text-align:center;">$m \leq$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 11$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$2000$</td>
</tr>
<tr>
<td style="text-align:center;">$12 \sim 20$</td>
<td style="text-align:center;" rowspan="2">$1000$</td>
<td style="text-align:center;">$5000$</td>
</tr>
<tr>
<td style="text-align:center;">$21 \sim 25$</td>
<td style="text-align:center;">$2 \times 10^5$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21027/file/attachment.zip">样例数据下载</a></p>
