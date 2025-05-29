<p><strong> 由于某些原因本题仅支持 C++ 各版本语言的提交。 </strong></p>
<p>距离上一次 Pak Dengklek 在他的家中粉刷墙壁已经过了一段时间，所以他想重新粉刷一次。他家的墙壁由 N 段组成，它们从 $0$ 到 $N −1$ 编号. 本题中我们假设存在 $K$ 种不同的颜色，颜色用从 $0$ 到 $K −1$ 的整数表示（例如, 红色用 $0$ 表示, 蓝色用 $1$ 表示， 以此类推）。Pak Dengklek 希望用第 $C[i]$ 种颜色来粉刷第 $i$ 段的墙壁。</p>
<p>为了粉刷墙壁, Pak Dengklek 雇用了一家有 $M$ 个承包商的承包商公司，承包商从 $0$ 到 $M −1$ 编号。对 Pak Dengklek 来说不幸的是，承包商只愿意粉刷他们自己喜欢的 颜色。具体来说，第 $j$ 个承包商喜欢 $A[j]$ 种颜色，并且只想用下列颜色来粉刷墙壁：第 $B[j][0]$ 种颜色，第 $B[j][1]$ 种颜色，$\cdots$，或第 $B[j][A[j]−1]$ 种颜色。 </p>
<p>Pak Dengklek 可以给承包商公司提出一些要求。在单个要求中，Pak Dengklek 将 给出两个参数 $x$ 和 $y$, 其中 $0 \le x &lt; M$ , $0 \le y \le N − M$。承包商公司将会指派第 $((x + l)\ \bmod M)$ 个承包商粉刷第 $(y + l)$ 段墙壁，其中 $0 \le l &lt; M$。如果存在一个 $l$ 使 得第 $((x + l)\ \bmod M)$ 个承包商不喜欢第 $C[y + l]$ 种颜色，那么该要求将无效。</p>
<p>Pak Dengklek 需要为每个要求付费，因此他想知道为了使墙壁中每个段都能用自己预期的颜色粉刷，他至少要提出多少个要求，或是确认他的预期无法达到。每一段墙 壁可以被粉刷多次，但必须保证每次粉刷的颜色都是 Pak Dengklek 所预期的。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>paint.h</code> 头文件。</p>
<p>你必须实现 <code>minimumInstructions</code> 函数：</p>
<pre><code class="sh_cpp">int minimumInstructions(int N, int M, int K, std::vector&lt;int&gt; C, std::vector&lt;int&gt; A, std::vector&lt;std::vector&lt;int&gt;&gt; B)</code></pre>
<ul>
<li><p>$N$：一个整数表示墙壁的段数。</p>
</li>
<li><p>$M$：一个整数表示承包商的数量。</p>
</li>
<li><p>$K$：一个整数表示颜色的种数。</p>
</li>
<li><p>$C$：一个长度为 $N$ 的整数序列，表示每段墙壁预期的颜色。</p>
</li>
<li><p>$A$：一个长度为 $M$ 的整数序列，表示承包商喜欢的颜色数。</p>
</li>
<li><p>$B$：一个长度为 $M$ 的每个元素为序列的序列，表示承包商喜欢的具体颜色。</p>
</li>
</ul>
<p>该函数将被评测库恰好调用一次。</p>
<p>该函数必须返回一个整数，表示 Pak Dengklek 为了让墙壁按预期粉刷所需要提出的最小要求数；若预期无法达到则返回 $-1$。</p>
<h2>样例评测库</h2>
<p>按照如下格式读入数据。</p>
<p>$N\ M\ K$ </p>
<p>$C[0]\ C[1]\ \cdots \ C[N-1]$ </p>
<p>$A[0]\ B[0][0]\ B[0][1]\ \cdots \ B[0][A[0]-1]$</p>
<p>$A[1]\ B[1][0]\ B[1][1]\ \cdots \ B[1][A[1]-1]$</p>
<p>$\cdots$</p>
<p>$\cdots$</p>
<p>$A[M-1]\ B[M-1][0]\ B[M-1][1]\ \cdots \ B[M-1][A[M-1]-1]$</p>
<p>样例评测库将输出函数 <code>minimumInstructions</code> 的返回值。</p>


<pre><code class="language-input1">8 3 5
3 3 1 3 4 4 2 2
3 0 1 2
2 2 3
2 3 4
</code></pre>


<pre><code class="language-output1">3
</code></pre>

<h2>限制与约定</h2>
<p>对于 $0 \le k &lt; K$,令 $f(k)$ 表示喜欢第 $k$ 种颜色的承包商数量。</p>
<p>对于所有测试数据：</p>
<ul>
<li>$1 \le N \le 100000.$</li>
<li>$1 \le M \le \min(N,50000)$</li>
<li>$1 \le K \le 100000.$</li>
<li>$0 \le C[i] &lt; K$.</li>
<li>$1 \le A[j] \le K$</li>
<li>$0 \le B[j][0] &lt; B[j][1] &lt; ... &lt; B[j][A[j]−1] &lt; K$.</li>
<li>$\sum f(k)^2 \le 400000$.</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
<th>依赖的数据包</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">$f(k) \le 1$</td>
<td style="text-align:center;">12</td>
<td>1, 2, 3, 4</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$N \le 500,M \le \min(N,200),\sum f(k)^2 \le 1000$</td>
<td style="text-align:center;">15</td>
<td>1, 5</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$N \le 500,M \le \min(N,200)$</td>
<td style="text-align:center;">13</td>
<td>1, 2, 5, 6</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$N \le 20000,M \le \min(N,2000)$</td>
<td style="text-align:center;">23</td>
<td>1, 2, 3, 5, 6, 7</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">37</td>
<td>1, 2, 3, 4, 5, 6, 7, 8</td>
</tr>
</tbody>
</table>
</div>
<p><strong> 实际测试中，前 8 个 subtask 为数据包，后 5 个 subtask 为 5 个子任务。 </strong></p>
<p><strong>时间限制</strong>：$2 \texttt{s}$</p>
<p><strong>空间限制</strong>：$512 \texttt{MB}$</p>
<h2>　下载</h2>
<p><a href="./20959/file/attachment.zip">样例及测评库下载</a></p>
