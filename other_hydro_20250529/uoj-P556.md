<p><strong> 由于某些原因本题仅支持 C++ 各版本语言的提交。 </strong></p>
<p>印度尼西亚有 $N$ 个城市以及 $M$ 条双向道路，城市从 $0$ 到 $N −1$ 编号，道路从 $0$ 到 $M −1$ 编号。每条道路连接着两个不同的城市，第 $i$ 条道路连接第 $U[i]$ 个城市与第 $V [i]$ 个城市，汽车行驶这条道路将耗费 $W[i]$ 个单位汽油。通过这些道路，任意两个城市间能够互相到达。 </p>
<p>接下来的 $Q$ 天中, 每天会有一对城市希望建立政治关系。具体来说，第 $j$ 天，第 $X[j]$ 个城市想要和第 $Y [j]$ 个城市建立政治关系。为此，第 $X[j]$ 个城市将会派一名代表坐汽车前往第 $Y [j]$ 个城市。同样地，第 $Y [j]$ 个城市也会派一名代表坐汽车前往第 $X[j]$ 个城市。 </p>
<p>为了避免拥塞，两辆车不应在任何时间点碰面。更具体地，两辆车不能在同一个时间点出现在同一个城市。同样地，两辆车也不应该沿相反的方向同时行驶过同一条道路。 另外，汽车行驶过一条道路时必须完整经过道路并到达道路另一端的城市（换句话说， 汽车不允许在道路中间掉转方向）。但是，汽车可以多次到达一个城市或是多次经过一 条道路。此外，汽车可以在任何时间在任何城市等候。 </p>
<p>由于高燃料容量汽车的价格昂贵，两个城市都分别希望选择一条路线，使得两辆汽车所需的最大单位汽油容量最小。每个城市中都有加油站并且供油量是无限的，因此汽车所需的单位汽油容量实际上就是行驶过的道路中最大的单位汽油消耗量。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>swap.h</code> 头文件。</p>
<p>你必须实现 <code>init</code> 和 <code>getMinimumFuelCapacity</code> 函数。</p>
<pre><code class="sh_cpp">void init(int N, int M, std::vector&lt;int&gt; U, std::vector&lt;int&gt; V, std::vector&lt;int&gt; W)</code></pre>
<ul>
<li>$N$：一个整数表示城市数。</li>
<li>$M$：一个整数表示道路数。</li>
<li>$U$：一个长为 $M$ 的整数序列表示道路的第一个端点城市。</li>
<li>$V$：一个长为 $M$ 的整数序列表示道路的第二个端点城市。</li>
<li>$W$：一个长为 $M$ 的整数序列表示道路的汽油消耗。</li>
</ul>
<p>该函数将在所有 <code>getMinimumFuelCapacity</code> 的调用前被评测库恰好调用一次。</p>
<pre><code class="sh_cpp">int getMinimumFuelCapacity(int X, int Y)</code></pre>
<ul>
<li>$X$：一个整数表示第一个城市。  </li>
<li>$Y$：一个整数表示第二个城市。  </li>
<li>该函数必须返回一个整数，表示根据题目描述中的规则，两辆分别从第 $X$ 个城市与第 $Y$ 个城市出发要到达彼此城市的车，它们的单位汽油容量最大值的最小值。若无法满足题目规则则返回 $−1$。</li>
</ul>
<p>该函数将被评测库调用恰好 $Q$ 次。</p>
<h2>样例评测库</h2>
<p>样例评测库将读入以下格式的数据：</p>
<pre>N M
U[0] V[0] W[0]
U[1] V[1] W[1]
.
.
.
U[M-1] V[M-1] W[M-1]
Q
X[0] Y[0]
X[1] Y[1]
.
.
.
X[Q-1] Y[Q-1]</pre><p>对每个 <code>getMinimumFuelCapacity</code> 的调用，样例评测库会输出该函数的返回值。</p>


<pre><code class="language-input1">5 6
0 1 4
0 2 4
1 2 1
1 3 2
1 4 10
2 3 3
3
1 2
2 4
0 1
</code></pre>


<pre><code class="language-output1">3
10
4
</code></pre>


<p><img src="//img.uoj.ac/problem/556/556_ex1.png" alt="样例一" class="img-responsive center-block" style="width:300px;"></p>
<h2>样例二</h2>
<p>见下载文件中的 <code>ex_swap2.in</code> 与 <code>ex_swap2.ans</code>。对应的图如下：</p>
<p><img src="//img.uoj.ac/problem/556/556_ex2.png" alt="样例二" class="img-responsive center-block" style="width:200px;"></p>
<h2>数据范围</h2>
<p>对于 $100\%$ 的数据，保证：</p>
<ul>
<li>$2 \leq N \leq 10^5$</li>
<li>$N − 1 \leq M \leq 2 \times 10^5$</li>
<li>$0 \leq U[i] &lt; V [i] &lt; N$</li>
<li>任意两个城市间至多存在一条道路直接相连。</li>
<li>任意两个城市经过道路可以互相到达。</li>
<li>$1 \leq W[i] \leq 10^9$</li>
<li>$1 \leq Q \leq 2 \times 10^5$</li>
<li>$0 \leq X[j] &lt; Y [j] &lt; N$</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
<th style="text-align:center;">　依赖的数据包</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">每个城市至多是两条道路的一个端点。</td>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">1, 2, 3, 4, 9</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$M = N − 1, U[i] = 0$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">1, 5</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$Q\le 5, N\le 1000, M\le 2000$</td>
<td style="text-align:center;">$17$</td>
<td style="text-align:center;">1, 2, 6, 10</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$Q\le 5$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">1, 2, 3, 6, 7, 10, 11</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$M=N-1$</td>
<td style="text-align:center;">$23$</td>
<td style="text-align:center;">1, 2, 3, 4, 5, 6, 7, 8</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$ $</td>
<td style="text-align:center;">$27$</td>
<td style="text-align:center;">1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12</td>
</tr>
</tbody>
</table>
</div>
<p><strong> 实际测试中，前 12 个 subtask 为数据包，后 6 个 subtask 为 6 个子任务。 </strong></p>
<p><strong>时间限制</strong>：$2 \texttt{s}$</p>
<p><strong>空间限制</strong>：$512 \texttt{MB}$</p>
<h2>　下载</h2>
<p><a href="./20960/file/attachment.zip">样例及测评库下载</a></p>
