<p>小 W 有一棵 $n$ 个结点的树，树上的每一条边可能是轻边或者重边。接下来你需要对树进行 $m$ 次操作，在所有操作开始前，树上所有边都是轻边。操作有以下两种：</p>
<ol>
<li>给定两个点 $a$ 和 $b$，首先对于 $a$ 到 $b$ 路径上的所有点 $x$（包含 $a$ 和 $b$），你要将与 $x$ 相连的所有边变为轻边。然后再将 $a$ 到 $b$ 路径上包含的所有边变为重边。</li>
<li>给定两个点 $a$ 和 $b$，你需要计算当前 $a$ 到 $b$ 的路径上一共包含多少条重边。</li>
</ol>
<h2>输入格式</h2>
<p>本题有多组数据，输入数据第一行一个正整数 $T$，表示数据组数。</p>
<p>对于每组数据： 第一行包含两个整数 $n$ 和 $m$，其中 $n$ 表示结点数量，$m$ 表示操作数量。</p>
<p>接下来 $n-1$ 行，每行包含两个整数 $u, v$，表示树上的一条边。</p>
<p>接下来 $m$ 行，每行包含三个整数 $op_i, a_i, b_i$，描述一个操作，其中 $op_i=1$ 表示第 $1$ 类操作，$op_i=2$ 表示第 $2$ 类操作。</p>
<p>数据保证 $a_i \neq b_i$。</p>
<h2>输出格式</h2>
<p>对于每一次第 $2$ 类操作，输出一行一个整数表示答案。</p>


<pre><code class="language-input1">1
7 7
1 2
1 3
3 4
3 5
3 6
6 7
1 1 7
2 1 4
2 2 7
1 1 5
2 2 7
1 2 1
2 1 7
</code></pre>


<pre><code class="language-output1">1
3
2
1
</code></pre>


<p>第 1 次操作后，重边有：$(1, 3)$，$(3, 6)$，$(6, 7)$。</p>
<p>第 2 次操作，包含的重边有：$(1, 3)$。</p>
<p>第 3 次操作，包含的重边有：$(1, 3)$，$(3, 6)$，$(6, 7)$。</p>
<p>第 4 次操作，首先 $(1, 3)$，$(3, 6)$ 变为轻边，之后 $(1, 3)$，$(3, 5)$ 变为重边。</p>
<p>第 5 次操作，包含的重边有：$(1, 3)$，$(6, 7)$。</p>
<p>第 6 次操作，首先 $(1, 3)$ 变为轻边，之后 $(1, 2)$ 变为重边。</p>
<p>第 7 次操作，包含的重边有：$(6, 7)$。</p>
<h2>样例二</h2>
<p>见附加文件的 <code>ex_edge2.in</code> 与 <code>ex_edge2.ans</code>。</p>
<p>该样例约束与测试点 $3 \sim 6$ 一致。</p>
<h2>样例三</h2>
<p>见附加文件的 <code>ex_edge3.in</code> 与 <code>ex_edge3.ans</code>。</p>
<p>该样例约束与测试点 $9 \sim 10$ 一致。</p>
<h2>样例四</h2>
<p>见附加文件的 <code>ex_edge4.in</code> 与 <code>ex_edge4.ans</code>。</p>
<p>该样例约束与测试点 $11 \sim 14$ 一致。</p>
<h2>样例五</h2>
<p>见附加文件的 <code>ex_edge5.in</code> 与 <code>ex_edge5.ans</code>。</p>
<p>该样例约束与测试点 $17 \sim 20$ 一致。</p>
<h2>测试点约束</h2>
<p>对于所有测试数据，有 $T \leq 3, 1 \leq n, m \leq 10^5$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n, m \leq$</th>
<th style="text-align:center;">特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 6$</td>
<td style="text-align:center;">$5000$</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 8$</td>
<td style="text-align:center;" rowspan="3">${10}^5$</td>
<td style="text-align:center;">A, B</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 10$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 14$</td>
<td style="text-align:center;">B</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 16$</td>
<td style="text-align:center;">$2 \times 10^4$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 20$</td>
<td style="text-align:center;">${10}^5$</td>
</tr>
</tbody>
</table>
</div>
<p>特殊性质 A：树的形态是一条链。</p>
<p>特殊性质 B：第 $2$ 类操作给出的 $a_i$ 和 $b_i$ 之间有边直接相连。</p>
<p><strong>时间限制：$\require{cancel}\cancel{\texttt{1s}}\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{1GB}$</strong></p>
