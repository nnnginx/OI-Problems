<p>JOI 王国坐落于一个 $xy$ 平面上，王国里有 $N$ 座小城，分别编号为 $1\ldots N$，其中第 $i$ 个小城的坐标为 $(X_i, Y_i)$。</p>
<p>现在王国正筹划着在小城之间建 $K$ 条路，而连接两个不同的小城 $i$ 和 $j$ 将花费 $|X_i-X_j|+|Y_i-Y_j|$ 元。在这里我们认为「连接小城 $i$ 和 $j$」和「连接小城 $j$ 和 $i$」本质相同。</p>
<p>和往常一样，你成为了这个项目的主管。为了估算花费情况，你想了解连接一些小城所需的花费。在这 $\frac{N(N-1)}{2}$ 条可能的道路中，你想了解最便宜的 $K$ 条道路的花费。</p>
<p>你的任务是，给出小城的坐标以及 $K$ 值，编写一个程序计算最便宜的 $K$ 条道路的花费。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $N$, $K$。</p>
<p>接下来 $N$ 行每行两个整数 $X_i,~Y_i$。</p>
<h2>输出格式</h2>
<p>输出 $K$ 行，第 $k$ 行为第 $k$ 便宜的道路价格。</p>


<pre><code class="language-input1">3 2 
-1 0 
0 2
0 0
</code></pre>


<pre><code class="language-output1">1
2
</code></pre>


<p>小城 $1,~2,~3$ 的坐标分别为 $(-1,~0),~$$(0,2),~$$(0,0)$，有 $\frac{3\times 2}{2}=3$ 种道路。</p>
<ul>
<li>在小城 $1$ 和 $2$ 之间建设道路花费 $|(−1) − 0| + |0 − 2| = 3$ 元。</li>
<li>在小城 $1$ 和 $3$ 之间建设道路花费 $|(−1) − 0| + |0 − 0| = 1$ 元。</li>
<li>在小城 $2$ 和 $3$ 之间建设道路花费 $|0 − 0| + |2 − 0| = 2$ 元。</li>
</ul>
<p>建设道路的价格从便宜到贵分别是 $1,~2,~3$。因此第一行输出 $1$，第二行输出 $2$。
本输入满足子任务 $1, 4, 5, 6$ 的条件。</p>


<pre><code class="language-input2">5 4
1 -1
2 0
-1 0
0 2
0 -2
</code></pre>


<pre><code class="language-output2">2
2
3
3
</code></pre>


<p>由 $N=5$ 知有 $\frac{5\times 4}{2}=10$ 种道路。</p>
<p>建设道路的价格从便宜到贵分别是 $2, 2, 3, 3, 3, 3, 4, 4, 4, 4$。因此，前 $4$ 便宜的道路价格为 $2, 2, 3, 3$。</p>
<p>本输入满足子任务 $1, 4, 5, 6$ 的条件。</p>
<h2>样例三</h2>
<p>本输入满足子任务 $1, 2, 4, 5, 6$ 的条件。</p>

<pre><code class="language-input2">4 6
0 0
1 0
3 0
4 0
</code></pre>


<pre><code class="language-output2">1
1
2
3
3
4
</code></pre>

<h2>样例四</h2>
<p>本输入满足子任务 $1, 4, 5, 6$ 的条件。</p>

<pre><code class="language-input2">10 10
10 -8
7 2
7 -8
-3 -6
-2 1
-8 6
8 -1
2 4
6 -6
2 -1
</code></pre>


<pre><code class="language-output2">3
3
4
5
6
6
6
7
7
7
</code></pre>

<h2>限制与约定</h2>
<p>对于 $100\%$ 的测试数据，有 $2\le N\le 250000,~$$1\le K\le\min(250000, \frac{N(N-1)}{2}),~$$-10^9\le X_i,~Y_i\le 10^9,~$$(X_i,~Y_i)\neq (X_j,Y_j) (1\le i &lt; j\le N)$。</p>
<p>各子任务详情如下：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">分值</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">5</td>
<td style="text-align:center;">$N\le 10^3$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">6</td>
<td style="text-align:center;">$Y_i=0$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">7</td>
<td style="text-align:center;">$K=1$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">20</td>
<td style="text-align:center;">$K\le 10$</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">27</td>
<td style="text-align:center;">$N\le 10^5$</td>
</tr>
<tr>
<td style="text-align:center;">6</td>
<td style="text-align:center;">35</td>
<td style="text-align:center;">无特殊限制</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{10s}$</strong></p>
<p><strong>空间限制：$\texttt{2GB}$</strong></p>
<h2>下载</h2>
<p><a href="./21017/file/attachment.zip">样例数据下载</a></p>
