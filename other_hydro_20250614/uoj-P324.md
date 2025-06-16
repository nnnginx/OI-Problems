<p>根据沙纳玛（Shahnameh）中的古代波斯传说，Zal，传奇的波斯英雄，疯狂地爱上了 Kabul 王国的公主 Rudaba。在 Zal 向 Rudaba 求婚时，Rudaba 的父亲给他了一个挑战。</p>
<p>在波斯有 $n$ 个城市，标记为从 $0$ 到 $n-1$，以及 $m$ 条双向道路，标记为从 $0$ 到 $m-1$。每条道路连接两个不同的城市。每一对城市至多会被一条道路连接。有些道路是御道（royal roads），专用于皇室行驶，但这是保密的。Zal 的任务是找出哪些道路是御道。</p>
<p>Zal 有一张包括所有城市和所有道路的波斯地图。他不知道哪些道路是御道，但是他可以求救于 Simurgh——好心的神鸟、Zal 的保护者。然而，Simurgh 并不想直接告诉他哪些道路是御道。作为替代，Simurgh 告诉 Zal，所有御道的集合是一个黄金集合（golden set）。一个道路的集合是黄金集合，当且仅当：</p>
<ul>
<li>它恰好包含 $n-1$ 条道路，而且</li>
<li>对于每一对城市，仅沿着这个集合中的道路即可从其中一个城市抵达另外一个城市。</li>
</ul>
<p>此外，Zal 可以问 Simurgh 一些问题。对于每个问题：</p>
<ol>
<li>Zal 选出道路的一个黄金集合，然后</li>
<li>Simurgh 会告诉 Zal，在所选择的黄金集合中有多少条道路是御道。</li>
</ol>
<p>你的程序可以问 Simurgh 最多 $q$ 个问题，以此帮助 Zal 找出御道的集合。评测工具将扮演 Simurgh 的角色。</p>
<h2>实现细节</h2>
<p><strong>本题只支持C++。</strong></p>
<p>你需要实现下面的函数：</p>
<pre><code class="sh_cpp"> std::vector&lt;int&gt; find_roads(int n, std::vector&lt;int&gt; u, std::vector&lt;int&gt; v)</code></pre>
<ul>
<li>$n$：城市的数量，</li>
<li>$u$ 和 $v$：均为长度为 $m$ 的数组。对于所有 $0\leq i\leq m-1$，$u[i]$ 和 $v[i]$ 是被道路 $i$ 所连接的城市。</li>
<li>该函数需要返回一个长度为 $n-1$ 的数组，其中包括了所有御道的标号（可以以任意的顺序给出）。</li>
</ul>
<p>你的程序至多只能调用评测工具中的如下函数 $q$ 次：</p>
<pre><code class="sh_cpp"> int count_common_roads(std::vector&lt;int&gt; r)</code></pre>
<ul>
<li>$r$：长度为 $n-1$ 的数组，其中包括了一个黄金集合中的道路标号（可以以任意的顺序给出）。</li>
<li>该函数将返回 $r$ 中的御道数量。</li>
</ul>
<h2>例子</h2>
<p>评测工具调用 <code>find_roads(4, [0, 0, 0, 1, 1, 2], [1, 2, 3, 2, 3, 3])</code>。</p>
<p><img src="https://img.uoj.ac/problem/324/IOI2017-simurgh-desc.png" alt="例子" class="img-responsive center-block" style="width:600px;"></p>
<p>这个例子中有 $4$ 个城市和 $6$ 条道路。我们将连接城市 $a$ 和 $b$ 的道路表示为 $(a,b)$。这些道路按照下面的顺序被标为从 $0$ 到 $5$：$(0,1)$，$(0,2)$，$(0,3)$，$(1,2)$，$(1,3)$ 和 $(2,3)$。每个黄金集合包含 $n-1=3$ 条道路。</p>
<p>假设御道是标号为 $0$，$1$ 和 $5$ 的道路，即 $(0,1)$，$(0,2)$ 和 $(2,3)$。这样的话：</p>
<p><code>count_common_roads([0, 1, 2])</code> 返回 $2$。该询问涉及到标号为 $0,1$ 和 $2$ 的道路，即 $(0,1)$，$(0,2)$ 和 $(0,3)$。其中有两条道路是御道。</p>
<p><code>count_common_roads([5, 1, 0])</code> 返回 $3$。该询问涉及到所有的御道。</p>
<p>函数 <code>find_roads</code> 需要返回 $[5,1,0]$ 或任意其他包含这三个元素且长度为 $3$ 的数组。</p>
<p>注意，下面列出的调用是不允许的：</p>
<ul>
<li><p><code>count_common_roads([0, 1])</code>：这里 $r$ 的长度不是 $3$。</p>
</li>
<li><p><code>count_common_roads([0, 1, 3])</code>：这里 $r$ 不是一个黄金集合，因为无法仅沿道路 $(0,1)$，$(0,2)$，$(1,2)$ 就从城市 $0$ 走到城市 $3$。</p>
</li>
</ul>
<h2>数据范围</h2>
<ul>
<li>$2\leq n\leq 500$</li>
<li>$n-1\leq m\leq n(n-1)/2$</li>
<li>$0\leq u[i],v[i]\leq n-1$（对于所有 $0\leq i\leq m-1$）</li>
<li>对于所有 $0\leq i\leq m-1$，道路 $i$ 连接两个不同的城市（即 $u[i]\neq v[i]$）。</li>
<li>每对城市之间至多连有一条道路。</li>
<li>经由这些道路，可以在任意一对城市之间来往。</li>
<li>所有的御道组成一个黄金集合。</li>
<li><code>find_roads</code> 可以调用 <code>count_common_roads</code> 最多 $q$ 次。在每次调用中，由 $r$ 所给出的道路必须是一个黄金集合。</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">$q=$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;" rowspan="3">$30000$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$13$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$17$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$240$</td>
<td style="text-align:center;">在任意两个城市之间都连有一条道路</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;" rowspan="2">$500$</td>
<td style="text-align:center;">$12000$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$19$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$8000$</td>
<td style="text-align:center;">$30$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$1024\texttt{MB}$</p>
<h2>评分程序样例</h2>
<p>评分程序样例将读入下述格式的输入数据：</p>
<ul>
<li>第 $1$ 行：$n\ m$</li>
<li>第 $2+i$ 行（对于所有 $0\leq i\leq m-1$）：$u[i]\ v[i]$</li>
<li>第 $2+m$ 行：$s[0]\ s[1]\ \cdots\ s[n-2]$</li>
</ul>
<p>这里 $s[0],s[1],\ldots,s[n-2]$ 是所有御道的标号。</p>
<p>如果 <code>find_roads</code> 最多调用 <code>count_common_roads</code> 了 $30000$ 次，而且正确地返回了御道的集合，评分程序样例将会输出 <code>YES</code>。否则评分程序样例将会输出 <code>NO</code>。</p>
<p>需要明确的是，评分程序样例中的函数 <code>count_common_roads</code> 不会检查 $r$ 是否满足一个黄金集合的所有条件。替代性地，它会对数组 $r$ 中的御道进行计数，并且返回。然而，在你提交的程序调用 <code>count_common_roads</code> 时，如果传给它的不是对应某个黄金集合的标号集合，评测结果将会是 <code>Wrong Answer</code>。</p>
<h2>hack</h2>
<p>在 <code>hack</code> 时，数据格式与上述类似，但是您需要在第 $1$ 行最后额外添加询问次数限制 $q$，这里要求 $q\in \{8000,12000,30000\}$。</p>
<h2>技术提示</h2>
<p>出于效率方面的考虑，函数 <code>count_common_roads</code> 使用了传引用调用（call by reference）的方式。你可以与平常一样调用这个函数。评测工具确保不会改变 $r$ 中的值。</p>
<h2>下载</h2>
<p><a href="./20750/file/attachment.zip">样例数据与样例评测库下载</a></p>
