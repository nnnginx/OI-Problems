<p>小 L 有一个有向图，图中的顶点可以分为 $k$ 层，第 $i$ 层有 $n_i$ 个顶点，第 $1$ 层与第 $k$ 层<strong>顶点数相同</strong>，即 $n_1=n_k$，且对于第 $j$（$2 \leq j \leq k-1$） 层，$n_1 \leq n_j \leq 2n_1$。对于第 $j$（$1 \leq j &lt; k$） 层的顶点，以它们为起点的边只会连向第 $j+1$ 层的顶点。没有边连向第 $1$ 层的顶点，第 $k$ 层的顶点不会向其他顶点连边。</p>
<p>现在小 L 要从这个图中选出 $n_1$ 条路径，每条路径以第 $1$ 层顶点为起点，第 $k$ 层顶点为终点，并要求<strong>图中的每个顶点至多出现在一条路径中</strong>。更具体地，把每一层顶点按照 $1, 2, \cdots, n_i$ 进行编号，则每条路径可以写为一个 $k$ 元组 ，表示这条路径依次经过第 $j$ 层的 $p_j$（$1 \leq p_j \leq n_j$）号顶点，并且第 $j$（$1 \leq j &lt; k$）层的 $p_j$ 号顶点有一条边连向第 $j+1$ 层的第 $p_{j+1}$ 号顶点。</p>
<p>小 L 把这些路径画在了纸上，发现它们会产生若干个交点。对于两条路径 $P, Q$，分别设它们在第 $j$ 层与第 $j+1$ 层之间的连边为 $(P_j, P_{j+1})$ 与 $(Q_j, Q_{j+1})$，若，</p>
<p>$$(P_j-Q_j) \times (P_{j+1}-Q_{j+1}) &lt; 0$$</p>
<p>则称它们在第 $j$ 层后产生了一个交点。两条路径的交点数为它们在第 $1, 2, \cdots, n$ 层后产生的交点总数。对于整个路径方案，它的交点数为 <strong>两两不同路径间交点数之和</strong> 。例如下图是一个 $3$ 条路径，共 $3$ 个交点的例子，其中红色点是交点。</p>
<p><img src="https://img.uoj.ac/problem/674/1.png" alt="例子" class="img-responsive center-block"></p>
<p>小 L 现在想知道有偶数个交点的路径方案数比有奇数个交点的路径方案数多多少个。两个路径方案被视为相同的，当且仅当它们的 $n_1$ 条路径按第一层起点编号顺序写下的 $k$ 元组能对应相同。由于最后的结果可能很大，请你输出它对 $998244353$（一个大质数）取模后的值。</p>
<h2>输入格式</h2>
<p>本题有多组数据，输入数据第一行一个正整数 $T$，表示数据组数。对于每组数据：</p>
<p>第一行一个正整数 $k$，表示一共有 $k$ 层顶点。</p>
<p>第二行包含 $k$ 个整数 $n_1, n_2, \cdots, n_k$，依次表示每一层的顶点数量。保证 $n_1=n_k$，且 $n_1 \leq n_i \leq 2n_1$（$2 \leq i \leq k-1$）。</p>
<p>第三行包含 $k-1$ 个整数 ，依次表示第 $j$ 层顶点到第 $j+1$ 层顶点的边数。保证 $m_j \leq n_j \times n_{j+1}$。</p>
<p>接下来有 $k-1$ 段输入。第 $j$（$1 \leq j &lt; k$）段输入包含 $m_j$ 行，每一行两个整数 $u, v$，表示第 $j$ 层的 $u$ 号顶点有一条边连向第 $j+1$ 层的 $v$ 号顶点。</p>
<p>数据保证图中不会出现重边。</p>
<h2>输出格式</h2>
<p>输出共 $T$ 行，每行一个整数，表示该组数据的答案对 $998244353$ 取模后的值。</p>


<pre><code class="language-input1">1
3
2 3 2
4 4
1 1 
1 2
2 1
2 3
1 2
2 1
3 1
3 2
</code></pre>


<pre><code class="language-output1">1
</code></pre>


<p>偶数个交点的方案有 $2$ 个，奇数个交点的方案有 $1$ 个，所以答案为 $1$。</p>
<p>将下表中路径 $1$ 和路径 $2$ 的方案交换，将会得到相同的方案，例如路径 $1$ 为 $(2, 3, 1)$ 且路径 $2$ 为 $(1, 1, 2)$ 的方案与方案 $1$ 是相同的方案，所以不会被计入答案。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">路径方案</th>
<th style="text-align:center;">路径 $1$</th>
<th style="text-align:center;">路径 $2$</th>
<th style="text-align:center;">交点总数</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$(1, 1, 2)$</td>
<td style="text-align:center;">$(2, 3, 1)$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$(1, 2, 1)$</td>
<td style="text-align:center;">$(2, 1, 2)$</td>
<td style="text-align:center;">$2$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$(1, 2, 1)$</td>
<td style="text-align:center;">$(2, 3, 2)$</td>
<td style="text-align:center;">$0$</td>
</tr>
</tbody>
</table>
</div>
<h2>样例二，样例三，样例四</h2>
<p>见附加文件下载。</p>
<h2>数据范围</h2>
<p>对于所有测试数据：$2 \leq k \leq 100$，$2 \leq n_1 \leq 100$，$1 \leq T \leq 5$。</p>
<p>每个测试点中，保证 $n_1 &gt; 10$ 的数据只有 $1$ 组。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$k=$</th>
<th style="text-align:center;">$n_1\leq$</th>
<th style="text-align:center;">特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$10$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 6$</td>
<td style="text-align:center;" rowspan="3">$10$</td>
<td style="text-align:center;">A,B</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 8$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 10$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 13$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$100$</td>
</tr>
<tr>
<td style="text-align:center;">$14 \sim 15$</td>
<td style="text-align:center;" rowspan="3">$100$</td>
<td style="text-align:center;">A,B</td>
</tr>
<tr>
<td style="text-align:center;">$16 \sim 17$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$18 \sim 20$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p>特殊性质 A：对于所有 $i$（$2 \leq i \leq k-1$）满足 $n_i=n_1$。</p>
<p>特殊性质 B：保证路径方案总数至多为 $1$。</p>
<p><strong>时间限制: $\require{cancel}\cancel{\texttt{1s}}\texttt{2s}$</strong></p>
<p><strong>空间限制: $\texttt{1GB}$</strong></p>
