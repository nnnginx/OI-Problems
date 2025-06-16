<p>要想打好松活弹抖闪电鞭，就得先掌握三维立体混元劲。</p>
<p>马老师是一名高维太极武术大师，根据他在 $k$ 维空间教人打拳的经历，他指出，你作为一名 $k$ 维生物，身上有 $n_1+\dots+n_k$ 处穴位，其中有 $n_j$ 处穴位来自第 $j$ 个维度。要想练好 $k$ 维立体混元劲，必先打通经脉，也就是说这 $n_1+\dots+n_k$ 处穴位通过经脉两两连通。也就是说如果将穴位看成点，穴位之间的经脉看成边，那么需要构成<strong>连通图</strong>。已知对于两个分别处于 $i,j$ 维度的穴位，打通这两个穴位有 $a_{i,j}$ 种方法。注意<strong>处于同一个维度的穴位之间也可以打通，但一个穴位不能和自己打通</strong>。</p>
<p>请你自行计算一下，有多少种方法可以给你打通经脉。由于方案数很多，你只需要算出同余 $998244353$ 的结果。</p>
<h2>输入格式</h2>
<p>第一行包含一个正整数 $k$，表示你所处的空间维度。</p>
<p>接下来一行输入 $k$ 个正整数，第 $j$ 个表示 $n_j$，即你在第 $j$ 个维度的穴位数量。</p>
<p>接下来输入 $k$ 行，每行 $k$ 个整数，其中第 $i$ 行第 $j$ 个数表示 $a_{i,j}$，保证 $a_{i,j}=a_{j,i}$。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，表示打通经脉的方案数，同余 $998244353$ 的结果。</p>


<pre><code class="language-input1">2
2 1
1 2
2 1
</code></pre>


<pre><code class="language-output1">12
</code></pre>


<p>共有 $2+1=3$ 个节点，其中 $(1,2)$ 间有 $1$ 种方式打通，$(1,3),(2,3)$ 各有 $2$ 种方式打通。</p>
<p>若 $(1,2)$ 间打通，那么接下来有 $(2+1)^2-1=8$ 种方式打通。</p>
<p>若 $(1,2)$ 间未打通，那么 $(1,3),(2,3)$ 必须各自打通，有 $2\times 2 = 4$ 种方式。</p>
<p>总共有 $8+4=12$ 种方式。</p>


<pre><code class="language-input2">2
7 4
1 998244352
998244352 0
</code></pre>


<pre><code class="language-output2">188336
</code></pre>

<h2>限制与约定</h2>
<p>记 $N=(n_1+1)\times \dots \times(n_k+1)$。</p>
<p>对于 $100\%$ 的数据，保证 $N\le 2.5\times 10^5, 0\le a_{i,j} &lt; 998244353$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">特殊限制</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$N\le 1000$</td>
<td style="text-align:center;">$10$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$k=1$</td>
<td style="text-align:center;">$10$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$k \le 2$</td>
<td style="text-align:center;">$15$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">$k\le 3$</td>
<td style="text-align:center;">$10$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">$n_j=1$</td>
<td style="text-align:center;">$15$</td>
</tr><tr><td style="text-align:center;">$6$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$40$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$4\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=596">样例数据下载</a></p>
