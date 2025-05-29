<p>Bob 喜欢线段树。</p>
<p>众所周知，ZJOI 的第二题有很多线段树。</p>
<p>Bob 有一棵根为 $[1, n]$ 的<strong>广义线段树</strong>。Bob 需要在这个线段树上执行 $k$ 次区间<strong>懒标记</strong>操作，每次操作会等概率地从 $[1, n]$ 的所有 $\frac{n(n+1)}2$ 个子区间中随机选择一个。对于所有在该次操作中被访问到的非叶子节点，Bob 会将这个点上的标记下推；而对于所有叶子节点（即没有继续递
归的节点），Bob 会给这个点打上标记。</p>
<p>Bob 想知道，$k$ 次操作之后，有标记的节点的期望数量是多少。</p>
<h4>具体定义</h4>
<p><strong>线段树</strong>：线段树是一棵每个节点上都记录了一个线段的二叉树。根节点记录的线段是 $[1, n]$。</p>
<p>对于每个节点，若它记录的线段是 $[l, r]$ 且 $l\neq r$，取 $m = \lfloor \frac{l+r}2 \rfloor$，则它的左右儿子节点记录的线段分别是 $[l,m]$ 和 $[m + 1, r]$；若 $l = r$，则它是叶子节点。</p>
<p><strong>广义线段树</strong>：在广义的线段树中，$m$ 不要求恰好等于区间的中点，但是 $m$ 还是必须满足 $l\le m &lt; r$ 的。不难发现在广义的线段树中，树的深度可以达到 $O(n)$ 级别。</p>
<p>线段树的核心是<strong>懒标记</strong>，下面是一个带懒标记的广义线段树的伪代码，其中 <code>tag</code> 数组为懒标记：</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/467/segcode.webp" style="width:700px;" alt="伪代码"></p>
<p>注意，在处理叶子节点时，一旦他获得了一个标记，那么这个标记会一直存在。</p>
<p>你也可以这么理解题意：有一棵广义线段树，每个节点有一个 $m$ 值。一开始 <code>tag</code> 数组均为 $0$，Bob 会执行 $k$ 次操作，每次操作等概率随机选择区间 $[l, r]$ 并执行 <code>MODIFY(root, 1, n, l, r);</code>。</p>
<p>最后所有 <code>Node</code> 中满足 <code>tag[Node] = 1</code> 的期望数量就是需要求的值。</p>
<h2>输入格式</h2>
<p>第一行输入两个整数 $n, k$。</p>
<p>接下来输入一行包含 $n − 1$ 个整数 $a_i$：按照<strong>先序遍历</strong>的顺序，给出广义线段树上所有非叶子节点的划分位置 $m$。你也可以理解为从只有 $[1, n]$ 根节点开始，每次读入一个整数后，就将当前包含这个整数的节点做一次拆分，最后获得一棵有 $2n − 1$ 个节点的广义线段树。</p>
<p>保证给定的 $n − 1$ 个整数是一个排列，不难发现通过这些信息就能唯一确定一棵 $[1, n]$ 上的广义线段树。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，代表期望数量对 $p = 998244353$ 取模后的结果。即，如果期望数量的最简分数表示为 $\frac ab$，你需要输出一个整数 $c$ 满足 $c\times b \equiv a \pmod p$。</p>


<pre><code class="language-input1">3 1
1 2
</code></pre>


<pre><code class="language-output1">166374060
</code></pre>


<p>输入的线段树为 $[1, 3], [1, 1], [2, 3], [2, 2], [3, 3]$。</p>
<p>若操作为 $[1, 1]/[2, 2]/[3, 3]/[2, 3]/[1, 3]$，标记个数为 $1$。若操作为 $[1, 2]$，标记个数为 $2$。故答案为 $\frac 76$。</p>


<pre><code class="language-input2">5 4
2 1 3 4
</code></pre>


<pre><code class="language-output2">320443836
</code></pre>

<h2>样例三</h2>
<p>见附加文件中 <code>ex_segment3.in</code> 与 <code>ex_segment3.ans</code>。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">测试点</th>
<th style="text-align:center;">$n$</th>
<th style="text-align:center;">$k$</th>
<th style="text-align:center;">其他约定</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$\le 10$</td>
<td style="text-align:center;">$\le 4$</td>
<td style="text-align:center;" rowspan="4">无</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$\le 10$</td>
<td style="text-align:center;">$\le 100$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$\le 5$</td>
<td style="text-align:center;">$\leq10^9$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">$\leq 200000$</td>
<td style="text-align:center;">$=1$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">$=32$</td>
<td style="text-align:center;" rowspan="6">$\leq10^9$</td>
<td style="text-align:center;" rowspan="3">输入的线段树为完全二叉树</td>
</tr><tr><td style="text-align:center;">$6$</td>
<td style="text-align:center;">$=64$</td>
</tr><tr><td style="text-align:center;">$7$</td>
<td style="text-align:center;">$=4096$</td>
</tr><tr><td style="text-align:center;">$8$</td>
<td style="text-align:center;">$\le 5000$</td>
<td style="text-align:center;">每个 $m$ 均在 $[l, r-1]$ 内均匀随机</td>
</tr><tr><td style="text-align:center;">$9$</td>
<td style="text-align:center;">$\le 100000$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr><tr><td style="text-align:center;">$10$</td>
<td style="text-align:center;">$\leq 200000$</td>
</tr></tbody></table></div>
<p>对于 $100\%$ 的数据，$1\le n\le 200000, 1\le k\le 10^9$。</p>
<p><strong>时间限制</strong>：$4\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20989/file/attachment.zip">样例数据下载</a></p>
