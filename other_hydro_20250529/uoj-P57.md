<p>在一个平面图中有 $n$ 个顶点和 $m$ 条直线段，第 $i$ 个顶点的坐标为 $(x_i, y_i)$，第 $j$ 条直线段连接顶点 $u_j$ 和顶点 $v_j$。权值为 $h_j$，除顶点 $u_j$ 和 $v_j$ 外直线段 $j$ 不经过其他的顶点。任意两条直线段如果存在公共点，则该公共点一定是一个顶点，此时这两条直线段都会连接这个顶点。对于任意的两个顶点 $x$ 和 $y$，总是可以找到一顶点序列 $a_1, a_2, \dots, a_k$ 使得 $a_1 = x, a_k = y$ 且对于任意 $1 \leq i &lt; k$ 满足 $a_i$ 和 $a_{i + 1}$ 被一条直线段直接连接。</p>
<p>这 $m$ 条直线段将整个平面分成了若干个区域，其中只有一个区域是无穷大的，其余均是有界的，我们称无穷大的区域为禁区。</p>
<p>现在给出 $q$ 次询问，每次给定平面中的任意两个不是顶点且分别不在任意一条直线段上的点 $A$ 和 $B$，请画一条<strong>曲线</strong>连接 $A$ 和 $B$，要求曲线不能经过禁区以及任何顶点，并使得穿过的直线段中权值最大的尽可能小。你需要对每次询问回答这个值最小为多少。</p>
<h2>输入格式</h2>
<p>第一行有两个正整数 $n, m$，分别表示顶点数和直线段数。</p>
<p>接下来 $n$ 行，每行两个整数，这部分中第 $i$ 行（总第 $i + 1$ 行）的两个整数 $x_i, y_i$ 为顶点 $i$ 的坐标。</p>
<p>接下来 $m$ 行，每行三个正整数 $u, v, h$，表示有一条直线段连接顶点 $u$ 和顶点 $v$，权值为 $h$。其中 $u \neq v$。</p>
<p>接下来一行，有一个正整数 $q$，表示询问数量。</p>
<p>接下来 $q$ 行，每行四个实数 $A_x, A_y, B_x, B_y$，表示一组两个点坐标分别为 $(A_x, A_y)$ 和 $(B_x, B_y)$ 的询问。</p>
<h2>输出格式</h2>
<p>输出 $q$ 行，每行一个正整数依次表示每个询问的答案。特别的，若不需要跨过任何一条边即可到达，请输出 $0$；若不存在合法的曲线，请输出 $-1$。</p>


<pre><code class="language-input1">9 12
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
1 2 10
2 3 10
3 6 10
6 9 10
9 8 10
8 7 10
7 4 10
4 1 10
2 5 3
5 8 2
5 6 4
4 5 1
3
1.5 1.5 2.5 2.5
1.5 2.5 2.5 1.5
0.5 0.5 1.5 1.5
</code></pre>


<pre><code class="language-output1">2
3
-1
</code></pre>

<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n, m, q$ 的范围</th><th>$x, y$ 的范围</th><th>其他特征</th></tr></thead><tbody><tr><td>1</td><td>$n = 10$，$m = 13$，$q = 20$</td><td rowspan="2">$0 \leq x \leq 1$，$0 \leq y \leq 2000$</td><td rowspan="5">所有直线段长度均等于 $1$</td></tr><tr><td>2</td><td>$n = 2012$，$m = 3016$，$q \leq 1000$</td></tr><tr><td>3</td><td>$n, m \leq 50$，$q \leq 200$</td><td rowspan="3">$0 \leq x,y \leq 1000$</td></tr><tr><td>4</td><td rowspan="2">$n, m \leq 100000$，$q \leq 100000$</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="2">$n, m \leq 2000$，$q \leq 2000$</td><td rowspan="5">$0 \leq x, y \leq 10^7$</td><td>每个有界区域都是凸多边形且每条直线段的权值均等于 $1$</td></tr><tr><td>7</td><td>每条直线段的权值均等于 $1$</td></tr><tr><td>8</td><td rowspan="3">$n, m \leq 100000$，$q \leq 100000$</td><td rowspan="3">无</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>对于全部数据，均满足 $5 \leq n, m \leq 100000$，所有直线段的权值不会超过 $10^9$。所有询问的坐标均为不超过 $10^7$ 的非负实数，且保证是 $0.5$ 的奇数倍。</p>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20497/file/attachment.zip">样例数据下载</a></p>
