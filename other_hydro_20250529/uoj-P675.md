<p>C 国是一个繁荣昌盛的国家，它由 $n$ 座城市和 $m$ 条有向道路组成，城市从 $1$ 到 $n$ 编号。如果从 $x$ 号城市出发，经过若干条道路后能到达 $y$ 号城市，那么我们称 $x$ 号城市可到达 $y$ 号城市，记作 $x \Rightarrow y$。C 国的道路有一个特点：对于三座城市 $x,~y,~z$，若 $x \Rightarrow z$ 且 $y \Rightarrow z$，那么有 $x \Rightarrow y$ 或 $y \Rightarrow x$。</p>
<p>再过一个月就是 C 国成立的千年纪念日，所以 C 国的人民正在筹备盛大的游行庆典。目前 C 国得知接下来会有 $q$ 次游行计划，第 $i$ 次游行希望从城市 $s_i$ 出发，经过若干个城市后，在城市 $t_i$ 结束，且在游行过程中，<strong>一个城市可以被经过多次</strong>。为了增加游行的乐趣，每次游行还会临时修建出 $k~(0 \leq k \leq 2)$ 条有向道路专门供本次游行使用， 即其他游行计划不能通过本次游行修建的道路。</p>
<p>现在 C 国想知道，每次游行计划可能会<strong>经过多少座城市</strong>。</p>
<p>注意：临时修建出的道路<strong>可以不满足 C 国道路原有的特点</strong>。</p>
<h2>输入格式</h2>
<p>第一行包含四个整数 $n,~m,~q,~k$，分别表示城市数、道路数、游行计划数以及每次游行临时修建的道路数。 </p>
<p>接下来 $m$ 行，每行包含两个整数 $u,~v$，表示一条有向道路 $u \rightarrow v$。</p>
<p>接下来 $q$ 行，每行前两个整数 $s_i, t_i$，表示每次游行的起点与终点；这行接下来有 $k$ 对整数 $a,~b$，每对整数表示一条临时添加的有向道路 $a \rightarrow b$。
数据保证，将 C 国原有的有向道路视为无向道路后，所有城市可以互达。</p>
<h2>输出格式</h2>
<p>对于每次询问，输出一行一个整数表示答案。如果一次游行从起点出发无法到达终点，输出 $0$ 即可。</p>


<pre><code class="language-input1">5 6 4 1
1 2
1 3
1 4
2 5
4 5
5 4
1 4 5 1
2 3 5 3
1 2 5 2
3 4 5 1
</code></pre>


<pre><code class="language-output1">4
4
4
0
</code></pre>


<p>第一次计划，起点为 $1$ 号点，终点为 $4$ 号点，临时修建道路为 $5 \rightarrow 1$，最终可能经过的城市编号为 ${1,~2,~4,~5}$。</p>
<p>第二次计划，起点为 $2$ 号点，终点为 $3$ 号点，临时修建道路为 $5 \rightarrow 3$，最终可能经过的城市编号为 ${2,~3,~4,~5}$。</p>
<p>第三次计划，起点为 $1$ 号点，终点为 $2$ 号点，临时修建道路为 $5 \rightarrow 2$，最终可能经过的城市编号为 ${1,~2,~4,~5}$。</p>
<p>第四次计划，起点为 $3$ 号点，终点为 $4$ 号点，临时修建道路为 $5 \rightarrow 1$，最终从 $3$ 号点出发无法到达 $4$ 号点。</p>
<h2>样例二</h2>
<p>见附加文件的 <code>celebration2.in</code> 与 <code>celebration2.ans</code>。</p>
<p>该样例约束与测试点 $5 \sim 7$ 一致。</p>
<h2>样例三</h2>
<p>见附加文件的 <code>celebration3.in</code> 与 <code>celebration3.ans</code>。</p>
<p>该样例约束与测试点 $10 \sim 11$ 一致。</p>
<h2>样例四</h2>
<p>见附加文件的 <code>celebration4.in</code> 与 <code>celebration4.ans</code>。</p>
<p>该样例约束与测试点 $15 \sim 16$ 一致。</p>
<h2>样例五</h2>
<p>见附加文件的 <code>celebration5.in</code> 与 <code>celebration5.ans</code>。</p>
<p>该样例约束与测试点 $20 \sim 25$ 一致。</p>
<h2>测试点约束</h2>
<p>对于 $100\%$ 的数据，有 $1\le n,~q \le 3\times 10^5,~$$n-1\le m\le 6\times 10^5,~$$0\le k\le 2$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n,~q\le$</th>
<th style="text-align:center;">$k$</th>
<th style="text-align:center;">特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$=0$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 7$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$\le 2$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$8 \sim 9$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=0$</td>
<td style="text-align:center;">$m=n-1$</td>
</tr>
<tr>
<td style="text-align:center;">$10 \sim 11$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=1$</td>
<td style="text-align:center;">$m=n-1$</td>
</tr>
<tr>
<td style="text-align:center;">$12 \sim 14$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=2$</td>
<td style="text-align:center;">$m=n-1$</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 16$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=0$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 19$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$20 \sim 25$</td>
<td style="text-align:center;">$3\times 10^5$</td>
<td style="text-align:center;">$=2$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\require{cancel}\cancel{\texttt{1s}}\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{1GB}$</strong></p>
