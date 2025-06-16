<p><strong> 由于某些原因本题仅支持 C++, C++11 语言的提交。 </strong></p>
<p>Ringo 正在参加在新加坡举办的一个嘉年华活动。他的口袋里装有一些奖券，这些奖券可以在嘉年华的游戏展位使用。假设共有 $n$ 种颜色的奖券，每张奖券涂上了其中的一种颜色并且印上了一个非负整数。不同奖券上的数字可能相同。依据嘉年华活动的规则要求，$n$ 保证是偶数。</p>
<p>Ringo 每种颜色的奖券有 $m$ 张，也就是说他共有 $n\cdot m$ 张奖券。其中，第 $i$ 种颜色对应的第 $j$ 张奖券上印的数字为 $x_{i,j}$（$0\le i\le n-1$ 且 $0\le j\le m - 1$）。</p>
<p>一次奖券游戏要进行 $k$ 轮，轮次的序号从 $0$ 到 $k-1$。每一轮按照下面的方式进行：</p>
<ul><li><p>首先，Ringo 从每种颜色的奖券中各选出一张奖券，形成一个 $n$ 张奖券的<strong>集合</strong>。</p>
</li>
<li><p>随后，游戏负责人记录下这个集合中奖券上的数字 $a_0, a_1, \dots, a_{n-1}$。不需要考虑这 $n$ 个整数的顺序。</p>
</li>
<li><p>接下来，游戏负责人从一个幸运抽奖箱中抽取一张特殊卡片，上面印有整数 $b$。</p>
</li>
<li><p>对于上述集合中每一个奖券上的数字 $a_i(0\le i \le n-1)$，游戏负责人会计算 $a_i$ 和 $b$ 的差的绝对值。让 $S$ 代表这 $n$ 个差的绝对值之和。</p>
</li>
<li><p>所得到的数字 $S$ 就是 Ringo 本轮能够获得的奖励数额。</p>
</li>
<li><p>一轮游戏结束后，本轮集合中的奖券全部被丢弃，不会在未来的轮次所使用。</p>
</li>
</ul><p>当 $k$ 轮游戏结束后，Ringo 会丢弃口袋中的所有奖券。</p>
<p>通过仔细观察，Ringo 发现这个奖券游戏被操控了！实际上，幸运抽奖箱里面内置了一台打印机。在每一轮，游戏负责人首先找到一个能够最小化当前轮次游戏奖励的整数 $b$，然后将该数字打印在他所抽取的特殊卡片上。</p>
<p>知道了这些信息之后，Ringo 想要设计每轮游戏中的奖券分配方案，使得 $k$ 轮游戏中获得的总体奖励数额之和最大。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>tickets.h</code> 头文件。</p>
<p>你需要实现下面这个函数：</p>
<pre><code class="sh_cpp">long long find_maximum(int k, std::vector&lt;std::vector&lt;int&gt;&gt; x)</code></pre>
<ul><li><p>$k$：游戏的轮数。</p>
</li>
<li><p>$x$：一个 $n\times m$ 的数组，记录了奖券上的数字。每种颜色的奖券按照上面的数字非递减顺序排序。</p>
</li>
<li><p>这个函数只会被调用一次。</p>
</li>
<li><p>这个函数应该只调用一次函数 <code>allocate_tickets</code>（参见下面的内容），它描述了 $k$ 轮游戏中的奖券分配方案，每一轮对应一个奖券集合。奖券的分配方案应该使得所获奖励数额之和达到最大。</p>
</li>
<li><p>这个函数需要返回能够获得的最大的奖励数额之和。</p>
</li>
</ul><p>函数 <code>allocate_tickets</code> 按照如下的方式进行定义：</p>
<pre><code class="sh_cpp">void allocate_tickets(std::vector&lt;std::vector&lt;int&gt;&gt; s)</code></pre>
<ul><li><p>$s$：一个 $n\times m$ 的数组。如果第 $i$ 种颜色的第 $j$ 张奖券如果被分配到了第 $r$ 轮游戏，那么 $s_{i,j}$ 的值应该为 $r$；如果未被使用，应该为 $-1$。</p>
</li>
<li><p>对于 $0\le i\le n-1$，在 $s_{i,0}, s_{i,1}, \dots, s_{i,m-1}$ 中，每个值 $0, 1, \dots, k - 1$ 必须只出现一次，而其他元素应该为 $-1$。</p>
</li>
<li><p>如果存在多种奖券分配方案能够达到最优的奖励数值，可以给出其中任何一种最优方案。</p>
</li>
</ul><h2>输入格式</h2>
<p>评测程序示例按照下面的格式读入数据：</p>
<ul><li>第 $1$ 行：$n\ m\ k$</li>
<li>第 $2 + i$ 行（$0\le i\le n-1$）：$x_{i, 0}\ x_{i,1}\ \dots\ x_{i,m-1}$</li>
</ul><h2>输出格式</h2>
<p>评测程序示例按照下面的格式打印你的答案：</p>
<ul><li>第 $1$ 行：<code>find_maximum</code> 的返回值</li>
<li>第 $2 + i$ 行（$0\le i\le n-1$）：$s_{i, 0}\ s_{i,1}\ \dots\ s_{i,m-1}$</li>
</ul>

<pre><code class="language-input1">2 3 2
0 2 5
1 1 3
</code></pre>


<pre><code class="language-output1">7
0 -1 1
-1 1 0
</code></pre>


<p>考虑下面的函数调用：</p>
<pre><code class="sh_cpp">find_maximum(2, [[0, 2, 5],[1, 1, 3]])</code></pre>
<p>这意味着：
- 游戏共进行 $k=2$ 轮；
- 第 $0$ 种颜色奖券上的整数数字分别是 $0, 2$ 和 $5$；
- 第 $1$ 种颜色奖券上的整数数字分别是 $1, 1$ 和 $3$；</p>
<p>一种能够获得最优奖励数值的分配方案是：</p>
<ul><li><p>在第 $0$ 轮，Ringo 选择第 $0$ 种颜色的第 $0$ 张奖券（印有整数 $0$）和第 $1$ 种颜色的第 $2$ 张奖券（印有整数$3$）。本轮获得的最小奖励数额是 $3$。例如，游戏负责人可以选择 $b=1$：$|1-0| + |1-3| = 1+2 = 3$。</p>
</li>
<li><p>在第 $1$ 轮，Ringo 选择第 $0$ 种颜色的第 $2$ 张奖券（印有整数 $5$）和第 $1$ 种颜色的第 $1$ 张奖券（印有整数 $1$）。本轮能够获得的最小奖励是 $4$。例如，游戏负责人可以选择 $b=3$：$|3-1|+|3-5|=2+2=4$。</p>
</li>
<li><p>因此，本次游戏两轮的奖励之和为 $3+4=7$。</p>
</li>
</ul><p>为了给出这个分配方案，函数 <code>find_maximum</code> 应该按照如下方式调用 <code>allocate_tickets</code>：</p>
<ul><li><code>allocate_tickets([[0, -1, 1], [-1, 1, 0]])</code></li>
</ul><p>最终，函数 <code>find_maximum</code> 应该返回数字 $7$。</p>


<pre><code class="language-input2">4 2 1
5 9
1 4
3 6
2 7
</code></pre>


<pre><code class="language-output2">12
-1 0
0 -1
0 -1
-1 0
</code></pre>

<h4>eplanation</h4>
<p>考虑下面的函数调用：</p>
<pre><code class="sh_cpp">find_maximum(1, [[5, 9], [1, 4], [3, 6], [2, 7]])</code></pre>
<p>这意味着：</p>
<ul><li>游戏只进行一轮；</li>
<li>第 $0$ 种颜色奖券上的数字分别是 $5$ 和 $9$；</li>
<li>第 $1$ 种颜色奖券上的数字分别是 $1$ 和 $4$；</li>
<li>第 $2$ 种颜色奖券上的数字分别是 $3$ 和 $6$；</li>
<li>第 $3$ 种颜色奖券上的数字分别是 $2$ 和 $7$；</li>
</ul><p>一种能够获得最优奖励的分配方案是：</p>
<ul><li>在第 $0$ 轮，Ringo 选择第 $0$ 种颜色的第 $1$ 张奖券（印有整数 $9$） ，第 $1$ 种颜色的第 $0$ 张奖券（印有整数 $1$），第 $2$ 种颜色的第 $0$ 张奖券（印有整数 $3$），第 $3$ 种颜色的第 $1$ 张奖券（印有整数 $7$）。本轮能够获得的最小奖励是 $12$。例如，游戏负责人可以选择 $b=3$：</li>
</ul><p>$$
|3-9| + |3-1| + |3-3| + |3-7| = 6 + 2 + 0 + 4 = 12
$$</p>
<p>为了给出这个分配方案，函数 <code>find_maximum</code> 应该按照如下方式调用 <code>allocate_tickets</code>：</p>
<ul><li><code>allocate_tickets([[-1, 0], [0, -1], [0, -1], [-1, 0]])</code></li>
</ul><p>最终，函数 <code>find_maximum</code> 应该返回数字 $12$。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，保证：</p>
<ul><li>$2\le n\le 1500$ 且 $n$ 为偶数</li>
<li>$1\le k\le m\le 1500$</li>
<li>$0\le x_{i,j}\le 10^9$（对于所有的 $0\le i\le n-1$ 且 $0\le j\le m-1$）</li>
<li>$x_{i,j-1}\le x_{i,j}$（对于所有的 $0\le i\le n-1$ 且 $1\le j\le m-1$）</li>
</ul><div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$m=1$</td>
<td style="text-align:center;">$11$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$k=1$</td>
<td style="text-align:center;">$16$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$0\le x_{i,j}\le 1$（对于所有的 $0\le i\le n-1$ 且 $0\le j\le m-1$）</td>
<td style="text-align:center;">$14$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">$k=m$</td>
<td style="text-align:center;">$14 $</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">$n,m\le 80$</td>
<td style="text-align:center;">$12$</td>
</tr><tr><td style="text-align:center;">$6$</td>
<td style="text-align:center;">$n,m\le 300$</td>
<td style="text-align:center;">$23$</td>
</tr><tr><td style="text-align:center;">$7$</td>
<td style="text-align:center;">没有其他限制</td>
<td style="text-align:center;">$10$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$2 \texttt{s}$</p>
<p><strong>空间限制</strong>：$1024 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20970/file/attachment.zip">样例及测评库下载</a></p>
