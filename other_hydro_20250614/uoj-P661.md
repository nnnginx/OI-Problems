<p><strong>由于某些原因本题仅支持 C++, C++11 语言的提交。</strong></p>
<p>建筑师 Timothy 设计了一个新的密室逃脱游戏。这个游戏里有 $n$ 个房间，房间从 $0$ 到 $n - 1$ 编号。最开始的时候，每个房间里都恰好有一把钥匙。每把钥匙都有一个类型，钥匙的类型是一个 $0$ 到 $n - 1$ 区间内的整数。第 $i$ 个房间里的钥匙类型是 $r[i]$。注意多个房间里可能会包含相同类型的钥匙，即 $r[i]$ 的值不一定是两两不同的。</p>
<p>游戏里还有 $m$ 条<strong>双向</strong>的通道，通道从 $0$ 到 $m - 1$ 编号。第 $j$ 条通道连接了⼀对编号不同的房间 $u[j]$ 和 $v[j]$。同一对房间之间可能存在多条通道。</p>
<p>参与游戏的玩家需要收集钥匙和在不同的房间之间通过通道进行移动。当玩家使用通道 $j$ 从房间 $u[j]$ 移动到 $v[j]$，或者反过来从 $v[j]$ 移动到 $u[j]$ 时，我们说玩家<strong>通过</strong>了通道 $j$。只有当玩家收集到类型为 $c[j]$ 的钥匙时，玩家才可以通过通道 $j$。</p>
<p>在游戏的任意时刻，玩家可以在某个房间 $x$ 里执行以下两种操作：</p>
<ul>
<li>收集房间 $x$ 里面的钥匙，钥匙的类型是 $r[x]$（除非对应类型的钥匙已经被收集过）。</li>
<li>通过通道 $j$，需要满足 $u[j] = x$ 或 $v[j] = x$，且玩家已经获得 $c[j]$ 类型的钥匙。</li>
</ul>
<p>注意玩家收集过的钥匙可以一直使用，<strong>永远不会被丢弃</strong>。</p>
<p>最初玩家会在某个房间 $s$ <strong>开始</strong>游戏，不带任何钥匙。如果玩家从房间 $s$ 开始，通过一系列上述描述的两种操作，能够到达房间 $t$，那么称房间 $t$ 是<strong>从房间 $\boldsymbol{s}$ 开始可以到达的</strong>。</p>
<p>对于每一个房间 $i$（$0 \le i \le n - 1$），定义从房间 $i$ 出发能够到达的房间数为 $p[i]$。Timothy 想要知道满足 $p[i]$ 值最小的下标 $i$ 的集合。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>keys.h</code> 头文件。</p>
<p>你要实现以下函数：</p>
<pre><code class="sh_cpp">int[] find_reachable(int[] r, int[] u, int[] v, int[] c)</code></pre>
<ul>
<li>$r$：一个长度为 $n$ 的序列。对于每一个 $i$（$0 \le i \le n - 1$），第 $i$ 个房间里的钥匙类型是 $r[i]$。</li>
<li>$u, v$：两个长度为 $m$ 的序列。对于每一个 $j$（$0 \le j \le m - 1$），第 $j$ 条通道连接了房间 $u[j]$ 和 $v[j]$。</li>
<li>$c$：一个长度为 $m$ 的序列。对于每一个 $j$（$0 \le j \le m - 1$），通过通道 $j$ 需要用到的钥匙类型是 $c[j]$。</li>
<li>这个函数应该返回一个长度为 $n$ 的序列 $a$。对于 $0 \le i \le n - 1$ 中的 $i$，如果满足 $p[i] \le p[j]$（$0 \le j \le n - 1$）那么 $a[i]$ 的值为 $1$，否则 $a[i]$ 的值为 $0$。</li>
</ul>
<h2>输入格式</h2>
<p>评测程序示例以如下格式读取输入数据：</p>
<ul>
<li>第 $1$ 行：$n \; m$</li>
<li>第 $2$ 行：$r[0] \; r[1] \; \ldots \; r[n - 1]$</li>
<li>第 $3 + j$ 行（$0 \le j \le m - 1$）：$u[j] \; v[j] \; c[j]$</li>
</ul>
<h2>输出格式</h2>
<p>样例评分程序按照以下格式打印 <code>find_reachable</code> 函数的返回值：</p>
<ul>
<li>第 $1$ 行：$s[0] \; s[1] \; \ldots \; s[n - 1]$</li>
</ul>


<pre><code class="language-input1">4 5
0 1 1 2
0 1 0
0 2 0
1 2 1
1 3 0
3 1 2
</code></pre>


<pre><code class="language-output1">0 1 1 0
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">find_reachable([0, 1, 1, 2],
               [0, 0, 1, 1, 3], [1, 2, 2, 3, 1], [0, 0, 1, 0, 2])</code></pre>
<p>如果玩家从房间 $0$ 开始游戏，可以执行以下的操作序列：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>当前房间</th>
<th>操作</th>
</tr>
</thead>
<tbody>
<tr>
<td>$0$</td>
<td>收集钥匙类型 $0$</td>
</tr>
<tr>
<td>$0$</td>
<td>通过通道 $0$ 到房间 $1$</td>
</tr>
<tr>
<td>$1$</td>
<td>收集钥匙类型 $1$</td>
</tr>
<tr>
<td>$1$</td>
<td>通过通道 $2$ 到房间 $2$</td>
</tr>
<tr>
<td>$2$</td>
<td>通过通道 $2$ 到房间 $1$</td>
</tr>
<tr>
<td>$1$</td>
<td>通过通道 $3$ 到房间 $3$</td>
</tr>
</tbody>
</table>
</div>
<p>因此从房间 $0$ 出发可以到达房间 $3$。类似地，我们可以构造出操作序列表明所有 $4$ 个房间都是从房间 $0$ 出发可达的，所以 $p[0] = 4$。下表展示了从各个房间出发可以到达的房间集合：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>开始房间 $i$</th>
<th>可以到达的房间</th>
<th>$p[i]$</th>
</tr>
</thead>
<tbody>
<tr>
<td>$0$</td>
<td>$[0,1,2,3]$</td>
<td>$4$</td>
</tr>
<tr>
<td>$1$</td>
<td>$[1,2]$</td>
<td>$2$</td>
</tr>
<tr>
<td>$2$</td>
<td>$[1,2] $</td>
<td>$2 $</td>
</tr>
<tr>
<td>$3$</td>
<td>$[1,2,3]$</td>
<td>$3$</td>
</tr>
</tbody>
</table>
</div>
<p>所有房间中 $p[i]$ 的最小值是 $2$，这可以在 $i = 1$ 或 $i = 2$ 处取得。所以这次函数调用的返回值是 $[0, 1, 1, 0]$。</p>


<pre><code class="language-input2">7 10
0 1 1 2 2 1 2
0 1 0
0 2 0
1 2 1
1 3 0
2 3 0
3 4 1
3 5 2
4 5 0
4 6 2
5 6 1
</code></pre>


<pre><code class="language-output2">0 1 1 0 1 0 1
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">find_reachable([0, 1, 1, 2, 2, 1, 2],
               [0, 0, 1, 1, 2, 3, 3, 4, 4, 5],
               [1, 2, 2, 3, 3, 4, 5, 5, 6, 6],
               [0, 0, 1, 0, 0, 1, 2, 0, 2, 1])</code></pre>
<p>下表展示了从各个房间出发可以到达的房间集合：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>开始房间 $i$</th>
<th>可以到达的房间</th>
<th>$p[i]$</th>
</tr>
</thead>
<tbody>
<tr>
<td>$0$</td>
<td>$[0, 1, 2, 3, 4, 5, 6]$</td>
<td>$7$</td>
</tr>
<tr>
<td>$1$</td>
<td>$[1, 2]$</td>
<td>$2$</td>
</tr>
<tr>
<td>$2$</td>
<td>$[1, 2]$ </td>
<td>$2$ </td>
</tr>
<tr>
<td>$3$</td>
<td>$[3, 4, 5, 6]$</td>
<td>$4$</td>
</tr>
<tr>
<td>$4$</td>
<td>$[4, 6]$</td>
<td>$2$</td>
</tr>
<tr>
<td>$5$</td>
<td>$[3, 4, 5, 6]$</td>
<td>$4$</td>
</tr>
<tr>
<td>$6$</td>
<td>$[4, 6]$</td>
<td>$2$</td>
</tr>
</tbody>
</table>
</div>
<p>所有房间中 $p[i]$ 的最小值是 $2$，这可以在 $i \in \{ 1, 2, 4, 6 \}$ 处取得。所以这次函数调用的返回值是 $[0, 1, 1, 0, 1, 0, 1]$。</p>


<pre><code class="language-input3">3 1
0 0 0
0 1 0
</code></pre>


<pre><code class="language-output3">0 0 1
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">find_reachable([0, 0, 0], [0], [1], [0])</code></pre>
<p>下表展示了从各个房间出发可以到达的房间集合：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>开始房间 $i$</th>
<th>可以到达的房间</th>
<th>$p[i]$</th>
</tr>
</thead>
<tbody>
<tr>
<td>$0$</td>
<td>$[0, 1]$</td>
<td>$2$</td>
</tr>
<tr>
<td>$1$</td>
<td>$[0, 1]$ </td>
<td>$2$ </td>
</tr>
<tr>
<td>$2$</td>
<td>$[2]$</td>
<td>$1$</td>
</tr>
</tbody>
</table>
</div>
<p>所有房间中 $p[i]$ 的最小值是 $1$，这可以在 $i = 2$ 处取得。所以这次函数调用的返回值是 $[0, 0, 1]$。</p>
<h2>数据范围</h2>
<p>对于所有数据：</p>
<ul>
<li>$2 \le n \le 3 \times {10}^5$</li>
<li>$1 \le m \le 3 \times {10}^5$</li>
<li>$0 \le r[i] \le n - 1$（对于所有的 $0 \le i \le n - 1$）</li>
<li>$0 \le u[j], v[j] \le n - 1$ 且 $u[j] \ne v[j]$（对于所有的 $0 \le j \le m - 1$）</li>
<li>$0 \le c[j] \le n - 1$（对于所有的 $0 \le j \le m - 1$）</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务</th>
<th style="text-align:center;">分值</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">$c[j] = 0$（对于所有的 $0 \le j \le m - 1$）且 $n, m \le 200$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$11$</td>
<td style="text-align:center;">$n, m \le 200$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$17$</td>
<td style="text-align:center;">$n, m \le 2000$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$30$</td>
<td style="text-align:center;">$c[j] \le 29$（对于所有的 $0 \le j \le m - 1$）且 $r[i] \le 29$（对于所有的 $0 \le i \le n - 1$）</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$33$</td>
<td style="text-align:center;">没有额外的约束条件</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{2GB}$</strong></p>
