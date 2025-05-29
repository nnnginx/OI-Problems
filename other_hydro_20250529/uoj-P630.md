<p>给定一张 $n$ 个点 $m$ 条边的有向图 $G$，其顶点从 $1 \sim n$ 编号。</p>
<p>对于任意两个点 $u, v$，若从顶点 $1$ 出发到达顶点 $v$ 的所有路径都需要经过顶点 $u$，则称顶点 $u$ 支配顶点 $v$。特别地，每个顶点支配其自身。</p>
<p>对于任意一个点 $v$，我们将图中支配顶点 $v$ 的顶点集合称为 $v$ 的受支配集 $D_v$。</p>
<p>现在有 $q$ 次互相独立的询问，每次询问给出一条有向边，请你回答在图 $G$ 中加入该条边后，有多少个顶点的受支配集发生了变化。</p>
<h2>输入格式</h2>
<p>第一行三个整数 $n, m, q$，分别表示图中的顶点数、边数，以及询问数。</p>
<p>接下来 $m$ 行每行两个整数 $x_i, y_i$，表示一条有向边 $x_i \rightarrow y_i$。</p>
<p>接下来 $q$ 行每行两个整数 $s_i, t_i$，表示每次询问加入的边 $s_i \rightarrow t_i$。</p>
<p>数据保证给出的图 $G$ 中，从 $1$ 号点出发能到达所有其他点，并且图中不包含重边与自环。</p>
<h2>输出格式</h2>
<p>对于每个询问输出一行一个整数表示答案。</p>


<pre><code class="language-input1">6 6 3
1 2
1 3
3 4
4 5
2 6
4 1
5 6
3 2
2 4
</code></pre>


<pre><code class="language-output1">1
0
2
</code></pre>


<p>对于原图，六个点的受支配集分别为：$D_1 = \{1\}, D_2 = \{1, 2\}, D_3 = \{1, 3\}, D_4 = \{1, 3, 4\}, D_5 = \{1, 3, 4, 5\}, D_6 = \{1, 2, 6\}$ 。</p>
<p>加入 $5 \rightarrow 6$ 后，$D_6 = \{1, 6\}$，其他点受支配集不变。</p>
<p>加入 $3 \rightarrow 2$ 后没有点受支配集改变。</p>
<p>加入 $2 \rightarrow 4 $ 后 $D_4 = \{1, 4\}, D_5 = \{1, 4, 5\}$，其他点受支配集不变。</p>
<h2>样例二</h2>
<p>见附加文件中 <code>ex_dominator2.in</code> 与 <code>ex_dominator2.ans</code>。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_dominator3.in</code> 与 <code>ex_dominator3.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试数据：$1 \leq n \leq 3000, 1 \leq m \leq 2 \times n, 1 \leq q \leq 2 \times 10^4$。</p>
<p>每个测试点的具体限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \leq$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 6$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$q \leq 100$</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 9$</td>
<td style="text-align:center;" rowspan="2">$1000$</td>
<td style="text-align:center;">$m = n - 1$</td>
</tr>
<tr>
<td style="text-align:center;">$10 \sim 15$</td>
<td style="text-align:center;">$q \leq 1000$</td>
</tr>
<tr>
<td style="text-align:center;">$16 \sim 20$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21031/file/attachment.zip">样例数据下载</a></p>
