<p>小 N 最近在研究 NP 完全问题，小 O 看小 N 研究得热火朝天，便给他出了一道这样的题目：</p>
<p>有 $n$ 个球，用整数 $1$ 到 $n$ 编号。还有 $m$ 个筐子，用整数 $1$ 到 $m$ 编号。</p>
<p>每个筐子最多能装 3 个球。</p>
<p>每个球只能放进特定的筐子中。具体有 $e$ 个条件，第 $i$ 个条件用两个整数 $v_i$ 和 $u_i$ 描述，表示编号为 $v_i$ 的球可以放进编号为 $u_i$ 的筐子中。</p>
<p>每个球都必须放进一个筐子中。如果一个筐子内有<strong>不超过</strong> $1$ 个球，那么我们称这样的筐子为<strong>半空</strong>的。</p>
<p>求半空的筐子最多有多少个，以及在最优方案中，每个球分别放在哪个筐子中。</p>
<p>小 N 看到题目后瞬间没了思路，站在旁边看热闹的小 I 嘿嘿一笑：“水题！”</p>
<p>然后三言两语道出了一个多项式算法。</p>
<p>小 N 瞬间就惊呆了，三秒钟后他回过神来一拍桌子：</p>
<p>“不对！这个问题显然是 NP 完全问题，你算法肯定有错！”</p>
<p>小 I 浅笑：“所以，等我领图灵奖吧!”</p>
<p>小 O 只会出题不会做题，所以找到了你——请你对这个问题进行探究，并写一个程序解决此题。</p>
<h2>输入格式</h2>
<p>第一行包含 $1$ 个正整数 $T$，表示有 $T$ 组数据。</p>
<p>对于每组数据，第一行包含 $3$ 个正整数 $n, m, e$，表示球的个数，筐子的个数和条件的个数。</p>
<p>接下来 $e$ 行,每行包含 $2$ 个整数 $v_i, u_i$，表示编号为 $v_i$ 的球可以放进编号为 $u_i$ 的筐子。</p>
<h2>输出格式</h2>
<p>对于每组数据，先输出一行，包含一个整数，表示半空的筐子最多有多少个。</p>
<p>然后再输出一行，包含 $n$ 个整数 $p_1, p_2, \dots , p_n$，相邻整数之间用空格隔开，表示一种最优解。其中 $p_i$ 表示编号为 $i$ 的球放进了编号为 $p_i$ 的筐子。如果有多种最优解,可以输出其中任何一种。</p>


<pre><code class="language-input1">1
4 3 6
1 1
2 1
2 2
3 2
3 3
4 3
</code></pre>


<pre><code class="language-output1">2
1 2 3 3
</code></pre>

<h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<p>对于所有数据，$T \leq 5$，$1 \leq n \leq 3m$。保证 $1 \leq v_i \leq n, 1 \leq u_i \leq m$，且不会出现重复的条件。</p>
<p>保证至少有一种合法方案,使得每个球都放进了筐子,且每个筐子内球的个数不超过 $3$。</p>
<p>各测试点满足以下约定:</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$m$</th>
<th>约定</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$\leq 10$</td><td rowspan="2">$n \leq 20$，$e \leq 25$</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="8">$\leq 100$</td><td>$e = nm$</td></tr><tr><td>4</td><td>存在方案使得有 $m$ 个半空的筐子</td></tr><tr><td>5</td><td rowspan="2">不存在有半空的筐子的方案</td></tr><tr><td>6</td></tr><tr><td>7</td><td rowspan="4">无</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20611/file/attachment.zip">样例数据下载</a></p>
