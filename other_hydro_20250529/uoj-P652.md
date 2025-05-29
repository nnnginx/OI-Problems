<p>在苏门答腊岛的热带雨林中，有 $N$ 棵树排成一排，从左到右依次用 $0$ 到 $N-1$ 进行编号，其中 $i$ 号树的高度为 $H[i]$，且所有树的高度互不相同。</p>
<p>PakDengklek 正在训练一只猩猩，让她能够从一棵树上跳到另一棵树上。对于一次跳跃，猩猩可以从一棵树，向左或向右跳到比当前这棵树高的第一棵树上。形式化地，如果猩猩当前在 $x$ 号树，那么当且仅当满足下列条件之一时，她能够跳到 $y$ 号树上：</p>
<ul>
<li>$y$ 是满足 $H[z]\gt H[x]$ 的所有 $z$ 中比 $x$ 小的最大非负整数；或者：</li>
<li>$y$ 是满足 $H[z]\gt H[x]$ 的所有 $z$ 中比 $x$ 大的最小非负整数。</li>
</ul>
<p>PakDengklek 有 $Q$ 个跳跃计划，每个计划用四个整数 $A,B,C$ 和 $D(A \le B \lt C \le D)$ 来描述。对于每个计划，PakDengklek 想知道猩猩是否能够从某棵树 $s\ (A \le s \le B)$ 出发，经过若干次跳跃，到达某棵树 $e\ (C \le e \le D)$。若该计划可行，PakDengklek 还想知道可行方案中猩猩需要的最少跳跃次数。</p>
<h2>实现细节</h2>
<p>你需要实现下列函数：</p>
<pre><code class="sh_cpp">void init(int N, int[] H)</code></pre>
<ul>
<li>$N$：树的数量。</li>
<li>$H$：大小为 $N$ 的数组，$H[i]$ 表示 $i$ 号树的高度。</li>
<li>该函数在第一次 <code>minimum_ jumps</code> 的调用前，将会被调用恰好一次。</li>
</ul>
<pre><code class="sh_cpp">int minimum_jumps(int A, int B, int C, int D)</code></pre>
<ul>
<li>$A,B$：可以用作起点的树的编号范围。</li>
<li>$C,D$：可以用作终点的树的编号范围。</li>
<li>该函数需要返回可行方案中猩猩需要的最少跳跃次数，或者返回 $−1$ 表示该计划不可行。</li>
<li>该函数将被调用恰好 $Q$ 次。</li>
</ul>
<h2>例子</h2>
<p>考虑如下调用：</p>
<pre>init(7, [3, 2, 1, 6, 4, 5, 7])
</pre>

<p>在初始化完成后，考虑如下调用</p>
<pre>minimum_jumps(4, 4, 6, 6)
</pre>

<p>该计划意味着猩猩必须从 $4$ 号树（高度为 $4$） 出发，并到达 $6$ 号树（高度为 $7$）。</p>
<p>一种跳跃次数最少的可行方案为：先跳到 $3$ 号树（高度为 $6$），再跳到 $6$ 号树。</p>
<p>另一种方案为：先跳到 $5$ 号树（高度为 $5$），再跳到 $6$ 号树。</p>
<p>因此，<code>minimum_jumps</code> 应该返回 $2$。</p>
<p>考虑另一个调用：</p>
<pre>minimum_jumps(1, 3, 5, 6)
</pre>

<p>该计划意味着猩猩必须从 $1$ 号树（高度为 $2$），$2$ 号树（高度为 $1$），或 $3$ 号树（高度为 $6$）之一出发，并最终到达 $5$ 号树（高度为 $5$）或者 $6$ 号树（高度为 $7$）。</p>
<p>唯一一种跳跃次数最少的可行方案为：从 $3$ 号树出发，直接跳到 $6$ 号树。</p>
<p>因此，<code>minimum_jumps</code> 应该返回 $1$。</p>
<p>考虑另一个调用：</p>
<pre>minimum_jumps(0, 1, 2, 2)
</pre>

<p>该计划意味着猩猩必须从 $0$ 号树（高度为 $3$）或者 $1$ 号树（高度为 $2$）出发，并最终到达 $2$ 号树（高度为 $1$）。</p>
<p>由于 $2$ 号树是高度最低的树，所以无法从其他树上跳到 $2$ 号树。</p>
<p>因此，<code>minimum_jumps</code> 应该返回 $-1$。</p>
<h2>输入格式</h2>
<p>示例测试程序按如下格式读取输入数据：</p>
<ul>
<li>第 $1$ 行：$N\ Q$</li>
<li>第 $2$ 行：$H[0]\ H[1]\ \cdots⋯ H[N-1]$</li>
<li>第 $3+i\ (0 \le i \le Q-1)$ 行：$A\ B\ C\ D$，表示第 $i$ 次 <code>minimum_jumps</code> 调用的参数。</li>
</ul>
<h2>输出格式</h2>
<p>示例测试程序按如下格式输出你的答案：</p>
<ul>
<li>第 $1+i\ (0 \le i \le Q-1)$ 行：第 $i$ 次 <code>minimum_jumps</code> 调用的返回值。</li>
</ul>
<h2>限制与约定</h2>
<p>对于所有数据：</p>
<ul>
<li>$2 \leq N \leq 200\ 000$</li>
<li>$1 \leq Q \leq 100\ 000$</li>
<li>$1 \leq H[i] \leq N (0 \leq i \leq N-1)$</li>
<li>$H[i] \neq H[j] (0 \leq i \lt j \leq N-1)$</li>
<li>$0 \leq A \leq B \lt C \leq D \leq N-1$</li>
</ul>
<p>子任务：</p>
<p><strong> 实际测试中，前 16 个 subtask 为数据包，后 7 个 subtask 为 7 个子任务。 </strong></p>
<ol>
<li>($4$ 分) $H[i]=i+1\ (0 \le i \le N−1)$</li>
<li>($8$ 分) $N,Q \le 200$</li>
<li>($13$ 分) $N,Q \le 2000$</li>
<li>($12$ 分) $Q \le 5$</li>
<li>($23$ 分) $A=B, C=D$</li>
<li>($21$ 分) $C=D$</li>
<li>($19$ 分) 无附加限制</li>
</ol>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./21053/file/attachment.zip">样例数据下载</a></p>
