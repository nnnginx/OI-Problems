<p>正当计算鸡们还沉浸在过年的气氛中时，计算鸡村拉响了警报：远方来了一群程序猿。“他们又要来了！” 全村上下陷入了惊恐。</p>
<p>看过了有手撕鬼子情节的抗日神剧的直径拆除鸡不禁开起了脑洞。作为一种神奇的生物，每个程序猿都长得十分古怪。人的身体形状可以抽象为一个五角星型的 $6$ 个结点的树，而程序猿则可以长成任意一个 $n$ 个结点的树。那么，如果每次能拆除这棵树的直径，最多要花费多少时间才能把这棵树全部删除呢？</p>
<p>具体来说，直径拆除鸡脑补的是这样一个算法：</p>
<ul><li>输入一棵 $n$ 个结点的树，该算法进行过程中保证每时每刻保证图是一个森林</li>
<li>令 $S = 0$，重复如下过程直到所有结点均被删除<ul><li>从图中任意找一个连通块，显然该连通块肯定是一棵树</li>
<li>假设该树有 $t$ 个结点，执行 $S = S + t$</li>
<li>从该树中找一条最长简单路，假设是从 $a$ 到 $b$。如果有多条那么选择 $a$ 最小的，当 $a$ 一样时选择 $b$ 最小的</li>
<li>删除从 $a$ 到 $b$ 的简单路上的所有结点，包括 $a$ 和 $b$，这将导致该树结点会被删光或者分裂成一个或多个更小的树</li>
</ul></li>
</ul><p>计算次数即最后 $S$ 所存储的值。</p>
<p>现在，给你 $n, m$，请你构造一个包含 $n$ 个结点的树，且计算次数至少为 $m$，输入数据保证有解。</p>
<h2>输入格式</h2>
<p>一行，两个整数 $n, m$。保证 $n \ge 1, m \ge 0$。</p>
<h2>输出格式</h2>
<p>$n - 1$ 行，每行两个整数 $v, u$ 表示树上一条从 $v$ 到 $u$ 的边，需要满足 $1 \le v, u \le n$。</p>


<pre><code class="language-input1">4 5
</code></pre>


<pre><code class="language-output1">1 2
1 3
1 4
</code></pre>


<p>输出了一个包含 $(1, 2), (1, 3), (1, 4)$ 三条边的四个结点的树。第一次直径拆除鸡将删除从 $2$ 到 $3$ 的简单路径上的所有结点，即 $\{2, 1, 3\}$，删除后仅剩一个结点，再花费 $1$ 的计算次数将其删除。总共 $S = 4 + 1 = 5$。</p>
<p>另外还有一种四个结点的方案，边分别是 $(1, 2), (2, 3), (3, 4)$。这棵树的最长简单路为 $\{1, 2, 3, 4\}$，所以第一次删除后所有结点均会被删除，总计算次数为 $4$，无法满足 $S \ge m$ 的条件。</p>


<pre><code class="language-input2">12 0
</code></pre>


<pre><code class="language-output2">1 2
2 3
1 4
4 5
1 7
6 7
7 8
1 10
10 9
10 11
10 12
</code></pre>

<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$n$</th>
<th>其它限制</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="3">$\leq 11$</td><td rowspan="3">无</td></tr><tr><td>2</td></tr><tr><td>3</td></tr><tr><td>4</td><td>$= 1023$</td><td>$m=3527$</td></tr><tr><td>5</td><td>$= 1023$</td><td>$m=11408$</td></tr><tr><td>6</td><td>$= 4095$</td><td>$m=93282$</td></tr><tr><td>7</td><td rowspan="4">$\le 10000$</td><td rowspan="4">无</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>对于所有数据，保证 $0 \le m \le 10^9$ 且保证有解。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20712/file/attachment.zip">样例数据下载</a></p>
