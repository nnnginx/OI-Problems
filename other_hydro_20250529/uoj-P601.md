<p>给定一张 $n$ 个点 $2 m$ 条边的有向图，图中的每条边上都有一个标记，代表一个左括号或者右括号。共有 $k$ 种不同的括号类型，即图中可能有 $2 k$ 种不同的标记。点、边、括号种类均从 $1$ 开始编号。</p>
<p>图中的每条边都会和另一条边成对出现。更具体地，若图中存在一条标有第 $w$ 种括号的左括号的边 $(u, v)$，则图中一定存在一条标有第 $w$ 种括号的右括号的边 $(v, u)$。同样地，图中每条标有右括号的边将对应着一条反方向的标有同类型左括号的边。</p>
<p>现在请你求出，图中共有多少个点对 $(x, y)$（$1 \le x &lt; y \le n$）满足：图中存在一条从 $x$ 出发到达 $y$ 的路径，且按经过顺序将路径各条边上的标记拼接得到的字符串是一个合法的括号序列。</p>
<h2>输入格式</h2>
<p>第一行三个整数 $n, m, k$，分别表示图中的点数，边对数和括号类型数。</p>
<p>接下来 $m$ 行，每行三个整数 $u, v, w$，表示一条从 $u$ 到 $v$ 的有向边，其标记为第 $w$ 种括号的左括号；以及一条从 $v$ 到 $u$ 的有向边，其标记为第 $w$ 种括号的右括号。</p>
<p>输入给出的图中，任意两个不同的顶点间可以有多条有向边相连，但图中不存在连向自身的有向边，即 $u \ne v$。</p>
<h2>输出格式</h2>
<p>输出仅一行一个整数，表示满足条件的点对数量。</p>


<pre><code class="language-input1">4 5 1
4 3 1
4 1 1
4 2 1
1 3 1
2 1 1
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>符合条件的点对及其对应的路径为：</p>
<p> $(1, 2)$：$1 \to 3 \to 4 \to 1 \to 2$。  </p>
<p> $(1, 4)$：$1 \to 3 \to 4$。  </p>
<p> $(2, 4)$：$2 \to 1 \to 4$。</p>


<pre><code class="language-input2">6 8 2
6 1 2
3 5 1
1 2 2
5 1 2
3 6 2
4 3 1
6 2 2
3 2 1
</code></pre>


<pre><code class="language-output2">10
</code></pre>

<h2>样例三</h2>
<p>见附加文件中 <code>ex_bracket3.in</code> 与 <code>ex_bracket3.ans</code>。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_bracket4.in</code> 与 <code>ex_bracket4.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试点：$1 \le n \le 3 \times {10}^5$，$1 \le m \le 6 \times {10}^5$，$1 \le k, u, v \le n$，$1 \le w \le k$。</p>
<p>每个测试点的具体限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n =$</th>
<th style="text-align:center;">$m \le$</th>
<th style="text-align:center;">$k \le$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="2">$2$</td>
<td style="text-align:center;" rowspan="3">无</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 8$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 12$</td>
<td style="text-align:center;" rowspan="2">$3000$</td>
<td style="text-align:center;">$6000$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 16$</td>
<td style="text-align:center;" rowspan="2">$n - 1$</td>
<td style="text-align:center;" rowspan="3">$n$</td>
<td style="text-align:center;" rowspan="2">不存在仅由带左括号标记的边构成的环</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 20$</td>
<td style="text-align:center;" rowspan="2">$3 \times {10}^5$</td>
</tr>
<tr>
<td style="text-align:center;">$21 \sim 25$</td>
<td style="text-align:center;">$6 \times {10}^5$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21005/file/attachment.zip">样例数据下载</a></p>
