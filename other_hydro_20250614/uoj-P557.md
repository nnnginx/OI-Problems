<p><strong> 由于某些原因本题仅支持 C++ 各版本语言的提交。 </strong></p>
<p>雅加达最大的主题公园中有 $N$ 个景点，它们从 $0$ 到 $N - 1$ 编号。这些景点由 $N - 1$ 条双向道路连接，任意两个景点间经由这些道路将存在唯一一条简单路径。道路从 $0$ 到 $N - 2$ 编号。第 $i$ 条道路连接第 $A_i$ 个景点与第 $B_i$ 个景点，经过这条道路需要花费一个小时。为了避免拥塞，每个景点将至多与三条道路相连。</p>
<p>你想寻找一条游玩路线并使得每个景点都被参观一次。你认为从一个景点走到下一个景点时经过太多道路是十分无聊的。为了寻找一条有趣的路线，你打算安排景点的参观顺序，使得参观下一个景点所花费的时间不超过参观之前景点所花费的时间。换句话说，你想找到一个序列 $P_0, P_1, \ldots, P_{N-1}$ 使其包含 $0$ 到 $N - 1$ 中的所有整数恰好一次，并且从第 $P_i$ 个景点到达第 $P_{i+1}$ 个景点所需的时间不超过从第 $P_{i-1}$ 个景点到达第 $P_i$ 个景点所需的时间，其中 $0 \lt i \lt N - 1$。</p>
<p>你手上没有景点的完整地图，因此你必须向信息中心进行若干次询问才能找到一条有趣路线。你最多能进行 $Q$ 次询问，每次询问需要提供两个参数 $X$ 和 $Y$，其中 $0 \le X, Y \lt N$。每次询问是以下任意一种：</p>
<p>从第 $X$ 个景点到第 $Y$ 个景点需要花费多少个小时。特别地，若 $X = Y$ 则回答将是 $0$。</p>
<p>有多少个景点 $Z$ 满足，当你想从第 $X$ 个景点到达第 $Z$ 个景点时一定会经过第 $Y$ 个景点。第 $Y$ 个景点将会被计算在内，特别地，若 $X = Y$ 则回答将是 $N$。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>fun.h</code> 头文件。</p>
<p>你必须实现 <code>createFunTour</code> 函数:</p>
<pre><code class="sh_cpp">std::vector&lt;int&gt; createFunTour(int N, int Q)</code></pre>
<p>该函数将被评测库恰好调用一次。</p>
<ul>
<li><p>$N$: 一个整数表示景点的数量。</p>
</li>
<li><p>$Q$: 一个整数表示询问次数的最大值。</p>
</li>
</ul>
<p>该函数可以调用以下两个交互函数：</p>
<pre><code class="sh_cpp">int hoursRequired(int X, int Y)</code></pre>
<ul>
<li>$X$: 一个整数表示第一个景点的编号。</li>
<li>$Y$: 一个整数表示第二个景点的编号。</li>
<li>该函数将返回一个整数表示从第 $X$ 个景点到第 $Y$ 个景点需要花费的小时数。</li>
<li>如果 $X$ 或 $Y$ 的值不在 $0$ 到 $N - 1$ 的范围内，该测试点将视为答案错误。</li>
</ul>
<pre><code class="sh_cpp">int attractionsBehind(int X, int Y)</code></pre>
<ul>
<li>$X$: 一个整数表示第一个景点的编号。</li>
<li>$Y$: 一个整数表示第二个景点的编号。</li>
<li>该函数将返回一个整数表示有多少个景点 $Z$ 满足，当你想从第 $X$ 个景点到达第 $Z$ 个景点时一定会经过第 $Y$ 个景点。</li>
<li>如果 $X$ 或 $Y$ 的值不在 $0$ 到 $N - 1$ 的范围内，该测试点将视为答案错误。</li>
<li>该函数必须返回一个长为 $N$ 的整数序列，表示你找到的景点参观顺序。</li>
</ul>
<h2>样例评测库</h2>
<p>样例评测库将读入以下格式的数据：</p>
<pre>N Q
A[0] B[0]
A[1] B[1]
.
.
.
A[N-2] B[N-2]</pre><p>如果 <code>createFunTour</code> 正确返回了一个满足题意的序列，并且 <code>hoursRequired</code> 和 <code>attractionsBehind</code> 的调用次数总和不超过 $Q$，那么样例评测库将会输出 <code>createFunTour</code> 得到的序列。其他情况下样例评测库将会输出错误信息。</p>


<pre><code class="language-input1">7 400000
0 1
0 5
0 6
1 2
1 4
2 3
</code></pre>


<pre><code class="language-output1">3 6 4 5 2 0 1
</code></pre>


<p>在下图的例子中 $N = 7$，$Q = 4\times 10^5$，$A = [0, 0, 0, 1, 1, 2]$，$B = [1, 5, 6, 2, 4, 3]$。</p>
<p><img src="//img.uoj.ac/problem/557/557_ex1.png" alt="样例一" class="img-responsive center-block" style="width:300px;"></p>
<p>评测库将调用 <code>createFunTour(7, 400000)</code>。</p>
<p>如果你询问 <code>hoursRequired(3, 5)</code>，函数将返回 $4$。
如果你询问 <code>hoursRequired(5, 4)</code>，函数将返回 $3$。
如果你询问 <code>attractionsBehind(5, 1)</code>，函数将返回 $4$。从第五个景点到第一、二、三、四个景点将一定会经过第一个景点。
如果你询问 <code>attractionsBehind(1, 5)</code>，函数将返回 $1$。
一个符合要求的返回序列为 $[3, 6, 4, 5, 2, 0, 1]$，到达下一个参观景点所需的时间按顺序分别为 $[4, 3, 3, 3, 2, 1]$。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，保证：</p>
<ul>
<li>$2 \le N \le 10^5$</li>
<li>$Q = 4\times 10^5$</li>
<li>任意两个景点间可以通过双向道路互相到达。</li>
<li>每个景点至多连接着三条道路。</li>
</ul>
<h4>子任务 $1$（$10$ 分）</h4>
<ul>
<li>$N \le 17$</li>
</ul>
<h4>子任务 $2$（$16$ 分）</h4>
<ul>
<li>$N \le 500$</li>
</ul>
<h4>子任务 $3$（$21$ 分）</h4>
<ul>
<li>对所有的 $1 \le i \lt N$，有一条连接着第 $i$ 个景点与第 $\left\lfloor\frac{i - 1}{2} \right\rfloor$ 个景点的双向道路。</li>
</ul>
<h4>子任务 $4$（$19$ 分）</h4>
<ul>
<li><p>存在至少一个景点 $T$ 使得对于所有 $0 \le i \lt N$，<code>hoursRequired(T, i)</code> $\lt 30$ 并且存在一个整数区间 $[L_i, R_i](0 \le L_i \le i \le R_i \lt N)$ 满足下列条件：</p>
<ul>
<li>从第 $T$ 个景点到达第 $j$ 个景点必须经过第 $i$ 个景点当且仅当 $L_i \le j \le R_i$。</li>
<li>若 $L_i \lt i$，则恰有一个景点 $X$ 满足：<ul>
<li>$L[i] \le X \lt i$</li>
<li>有一条连接第 $i$ 个景点与第 $X$ 个景点的道路。</li>
</ul>
</li>
<li>若 $i \lt R_i$，则恰有一个景点 $Y$ 满足：<ul>
<li>$i \lt Y \le R_i$</li>
<li>有一条连接第 $i$ 个景点与第 $Y$ 个景点的道路。</li>
</ul>
</li>
</ul>
</li>
</ul>
<h4>子任务 $5$（$34$ 分）</h4>
<ul>
<li>无附加限制。</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务</th>
<th style="text-align:center;">依赖的数据包</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">1, 2, 3, 4</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">1, 2, 3, 4, 5, 6, 7</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">1, 2, 5, 8</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">1, 3, 6, 9</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">1, 2, 3, 4, 5, 6, 7, 8, 9, 10</td>
</tr>
</tbody>
</table>
</div>
<p><strong> 实际测试中，前 10 个 subtask 为数据包，后 5 个 subtask 为 5 个子任务。 </strong></p>
<p><strong>时间限制</strong>：$2 \texttt{s}$</p>
<p><strong>空间限制</strong>：$512 \texttt{MB}$</p>
<h2>　下载</h2>
<p><a href="./20961/file/attachment.zip">样例及测评库下载</a></p>
