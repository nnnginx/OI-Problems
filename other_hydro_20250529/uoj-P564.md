<p><strong> 由于某些原因本题仅支持 C++, C++11 语言的提交。 </strong></p>
<p>植物学家 Hazel 参观过新加坡植物园的一个特别展览。在这次展览中，有 $n$ 棵高度互不相同的植物，它们排成了一个圆。这些植物按顺时针方向从 $0$ 到 $n-1$ 编号，植物 $n-1$ 与植物 $0$ 是相邻的。</p>
<p>对于每棵植物 $i\ (0\le i\le n-1 )$，Hazel 将它与顺时针方向的后 $k-1$ 棵植物进行比较，记录下数值 $r_i$ 以表示这 $k-1$ 棵植物中有多少棵的高度大于植物 $i$。因此，每个 $r_i$ 的数值是由某段连续 $k$ 棵植物的相对高度决定的。</p>
<p>例如，假设 $n=5$，$k=3$，$i=3$。植物 $3$ 顺时针方向的后 $k-1=2$ 棵植物是植物 $4$ 和植物 $0$。如果植物 $4$ 比植物 $3$ 高，且植物 $0$ 比植物 $3$ 矮，那么 Hazel 将会记录 $r_3 = 1$。</p>
<p>你可以假设 Hazel 记录的数值 $r_i$ 都是正确的。也就是说，这些植物至少存在一组互不相同的高度符合 Hazel 所记录的数值。</p>
<p>本题要求你比较 $q$ 对植物的高度。由于你没有机会参观这次展览，你仅有的信息来源是 Hazel 的笔记本，其中记录了 $k$ 和序列 $r_0,\ldots, r_{n-1}$ 的值。
对于每对需要比较的植物 $x$ 和 $y$（$x$ 和 $y$ 不同），判定它们符合以下哪种情况：</p>
<ul><li><p>植物 $x$ 一定比植物 $y$ 高：对于任意一组符合数组 $r$ 且互不相同的高度 $h_0,\ldots h_{n-1}$，都有 $h_x\gt h_y$。</p>
</li>
<li><p>植物 $x$ 一定比植物 $y$ 矮：对于任意一组符合数组 $r$ 且互不相同的高度 $h_0,\ldots h_{n-1}$，都有 $h_x\lt h_y$。</p>
</li>
<li><p>该比较没有定论：以上两种情况都不成立。</p>
</li>
</ul><h2>实现细节</h2>
<p>你必须引用 <code>plants.h</code> 头文件。</p>
<p>要求你实现以下函数：</p>
<pre><code class="sh_cpp">void init(int k, int[] r)</code></pre>
<ul><li>$k$：决定每个 $r_i$ 数值的连续植物的棵数。</li>
<li>$r$：一个大小为 $n$ 的数组，其中 $r_i$ 是植物 $i$ 顺时针方向的后 $k-1$ 棵植物中比它高的棵数。</li>
<li>该函数恰好被调用一次，且在对 <code>compare_plants</code> 的任何调用之前。</li>
</ul><pre><code class="sh_cpp">int compare_plants(int x, int y)</code></pre>
<ul><li>$x,y$：待比较的植物的编号。</li>
<li>该函数应该返回：<ul><li>$1$：如果植物 $x$ 一定比植物 $y$ 高，</li>
<li>$-1$：如果植物 $x$ 一定比植物 $y$ 矮，</li>
<li>$0$：如果该比较没有定论。</li>
</ul></li>
<li>该函数恰好被调用 $q$ 次。</li>
</ul><h2>输入格式</h2>
<p>评测程序示例以如下格式读取输入数据：</p>
<ul><li>第 $1$ 行：$n\ k\ q$</li>
<li>第 $2$ 行：$r_{0}\ r_{1}\ \ldots\ r_{n-1}$</li>
<li>第 $3+i\ (0\le i\le q-1)$ 行：$x\ y$，表示第 $i$ 次调用 <code>compare_plants</code> 时的参数</li>
</ul><h2>输入格式</h2>
<p>评测程序示例以如下格式打印你的答案：</p>
<ul><li>第 $1+i\ (0\le i\le q-1)$ 行: 第 $i$ 次调用 <code>compare_plants</code> 的返回值</li>
</ul>

<pre><code class="language-input1">4 3 2
0 1 1 2
0 2
1 2
</code></pre>


<pre><code class="language-output1">1
-1
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">init(3, [0, 1, 1, 2])</code></pre>
<p>假设评测程序调用了 <code>compare_plants(0, 2)</code>。由 $r_0=0$ 可以推断植物 $2$ 不比植物 $0$ 高，因此该调用应该返回 $1$。</p>
<p>假设评测程序接下来调用了 <code>compare_plants(1, 2)</code>。由于对每组符合以上条件的植物高度，都有植物 $1$ 比植物 $2$ 矮，因此该调用应该返回 $-1$。</p>


<pre><code class="language-input2">4 2 2
0 1 0 1
0 3
1 3
</code></pre>


<pre><code class="language-output2">1
0
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">​init(2, [0, 1, 0, 1])</code></pre>
<p>假设评测程序调用了 <code>compare_plants(0, 3)</code>。由 $r_3=1$ 可以推断植物 $0$ 比植物 $3$ 高，因此该调用应该返回 $1$。</p>
<p>假设评测程序接下来调用了 <code>compare_plants(1, 3)</code>。两组高度 $[3,1,4,2]$ 和 $[3,2,4,1]$ 都符合 Hazel 的观测记录，由于在第一种情况中植物 $1$ 比植物 $3$ 矮，而在第二种情况中它比植物 $3$ 高，因此该调用应该返回 $0$。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，满足：</p>
<ul><li>$2\le k\le n\le 200\ 000$</li>
<li>$1\le q\le 200\ 000$</li>
<li>$0\le r_i\le k-1$（对所有 $0\le i\le n-1$）</li>
<li>$0\le x\lt y\le n-1$</li>
<li>存在一组或多组<strong>互不相同的高度</strong>符合数组 $r$ 记录的情况</li>
</ul><div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$k=2$</td>
<td style="text-align:center;">$5$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$n\le 5000, 2\cdot k&gt;n$</td>
<td style="text-align:center;">$14$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$2\cdot k&gt;n$</td>
<td style="text-align:center;">$13$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">每次 <code>compare_plants</code> 调用的正确答案是 $1$ 或 $-1$</td>
<td style="text-align:center;">$17$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">$n\le 300, q\le \frac{n\cdot (n-1)}{2}$</td>
<td style="text-align:center;">$11$</td>
</tr><tr><td style="text-align:center;">$6$</td>
<td style="text-align:center;">每次调用 <code>compare_plants</code> 时有 $x=0$</td>
<td style="text-align:center;">$15$</td>
</tr><tr><td style="text-align:center;">$7$</td>
<td style="text-align:center;">没有附加约束条件</td>
<td style="text-align:center;">$25$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$4 \texttt{s}$</p>
<p><strong>空间限制</strong>：$1024 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20968/file/attachment.zip">样例及测评库下载</a></p>
