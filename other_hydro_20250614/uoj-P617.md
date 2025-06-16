<p><strong> 由于一些原因，本题空间限制由原题 $\texttt{4GB}$ 改为 $\texttt{2GB}$。</strong></p>
<p>JOI 街是一条贯通东西的长街。我们将其抽象为一条数轴。</p>
<p>从现在起，将有 $N$ 个贵宾（VIP）来到 JOI 街并大逛特逛。VIP 们以 $1$ 到 $N$ 编号。VIP $i\ (1 \le i \le N)$ 将会在时刻 $T_i$ 从坐标 $A_i$ 前往坐标 $B_i$。其速度是每单位时间 $1$ 单位长度。<br>如果 $A_i &lt; B_i$，VIP $i$ 将会以不变的速度在正方向上移动。类似地，如果 $A_i &gt; B_i$，VIP $i$ 将会以不变的速度在负方向上移动。</p>
<p>一个保镖的工作是在 JOI 街上巡逻并保护 VIP 们。为了保护一个 VIP，很有必要和 TA 一起逛一会街，同时保护 TA。当然，允许保镖在他们逛街逛到一半时才开始保护，或在他们逛街结束前就停止保护。开始和停止保护的时刻<strong>不必为一个整数</strong>。<br>特别地，尽管可能有多个 VIP 在同一坐标，保镖也最多只能保护一个 VIP。</p>
<p>保镖可以在 JOI 街上以每单位时间最多 $1$ 单位长度的速度随意走动。在他们停止保护一个 VIP 之后，可以去到另一个地方再开始保护另一个 VIP。如果一个保镖和 VIP $i$ 一起逛街，那么 VIP 将会对他们一起走过的距离的每单位长度给保镖 $C_i$ 元小费。这里保证 $C_i$ 是偶整数。</p>
<p>作为一个安保公司的员工，您正在计划 $Q$ 份保护 VIP 的方案。这些方案以 $1$ 到 $Q$ 编号。对于方案 $j\ (1 \le j \le Q)$，一个保镖在时刻 $P_j$ 时从坐标 $X_j$ 开始工作。您的任务是分别最大化每个方案中的保镖能够得到的总小费。</p>
<p>请您编写一个程序对于给定的 VIP 和保镖的信息，计算每一个方案中保镖的最大总小费。</p>
<p>在此题的限制下，可以证明答案一定是个整数。</p>
<h2>输入格式</h2>
<p>第一行，两个整数 $N,Q$。  </p>
<p>接下来 $N$ 行，每行四个整数 $T_i,A_i,B_i,C_i$。  </p>
<p>接下来 $Q$ 行，每行两个整数 $P_j,X_j$。</p>
<h2>输出格式</h2>
<p>输出 $Q$ 行。第 $j\ (1 \le j \le Q)$ 行应当包含一个整数表示方案 $j$ 中保镖能得到的最大总小费。</p>


<pre><code class="language-input1">2 2
1 2 1 4
3 1 3 2
1 2
3 3
</code></pre>


<pre><code class="language-output1">8
2
</code></pre>


<p>在方案 $1$ 中，一个保镖可以按照以下方式得到 $4+4=8$ 元。</p>
<ol>
<li>在时刻 $1$ 从坐标 $2$ 开始工作。</li>
<li>在时刻 $1$ 到时刻 $2$ 间保护 VIP $1$。由于他们一起走过了 $1$ 单位长度，他得到 $4 \times 1 = 4$ 元的小费。</li>
<li>在时刻 $2$ 到时刻 $3$ 间留在坐标 $1$。</li>
<li>在时刻 $3$ 到时刻 $5$ 间保护 VIP $2$。由于他们一起走过了 $2$ 单位长度，他得到 $2 \times 2 = 4$ 元的小费。</li>
</ol>
<p>由于这是最大值，所以第一行输出 $8$。</p>
<p>在方案 $2$ 中，一个保镖可以按照以下方式得到 $2$ 元。</p>
<ol>
<li>在时刻 $3$ 从坐标 $3$ 开始工作。</li>
<li>在时刻 $3$ 到时刻 $4$ 间从坐标 $3$ 移动到坐标 $2$。</li>
<li>在时刻 $4$ 到时刻 $5$ 间保护 VIP $2$。由于他们一起走过了 $1$ 单位长度，他得到 $2 \times 1 = 2$ 元的小费。</li>
</ol>
<p>由于这是最大值，所以第二行输出 $2$。</p>
<p>这组样例满足子任务 $1,3,4,5$ 的限制。</p>


<pre><code class="language-input2">3 2
3 1 5 2
1 4 1 4
4 2 4 4
2 2
6 3
</code></pre>


<pre><code class="language-output2">15
0
</code></pre>


<p>在方案 $1$ 中，一个保镖可以按照以下方式得到 $4+1+8+2=15$ 元。</p>
<ol>
<li>在时刻 $2$ 从坐标 $2$ 开始工作。</li>
<li>在时刻 $2$ 到时刻 $2.5$ 间从坐标 $2$ 移动到坐标 $2.5$。</li>
<li>在时刻 $2.5$ 到时刻 $3.5$ 间保护 VIP $2$。由于他们一起走过了 $1$ 单位长度，他得到 $4 \times 1 = 4$ 元的小费。</li>
<li>在时刻 $3.5$ 到时刻 $4$ 间保护 VIP $1$。由于他们一起走过了 $0.5$ 单位长度，他得到 $2 \times 0.5 = 1$ 元的小费。</li>
<li>在时刻 $4$ 到时刻 $6$ 间保护 VIP $3$。由于他们一起走过了 $2$ 单位长度，他得到 $4 \times 2 = 8$ 元的小费。</li>
<li>在时刻 $6$ 到时刻 $7$ 间保护 VIP $1$。由于他们一起走过了 $1$ 单位长度，他得到 $2 \times 1 = 4$ 元的小费。</li>
</ol>
<p>由于这是最大值，所以第一行输出 $15$。</p>
<p>在方案 $2$ 中，保镖在时刻 $6$ 从坐标 $3$ 开始工作。然而，TA 无法保护任何 VIP。因此最大总小费为 $0$ 元。因此第二行输出 $0$。</p>
<p>这组样例满足子任务 $1,3,4,5$ 的限制。</p>
<h2>样例三</h2>
<p>这组样例满足子任务 $1,3,4,5$ 的限制。</p>

<pre><code class="language-input2">5 5
8 1 4 10
8 3 7 6
1 4 6 2
3 9 5 4
6 1 9 6
7 6
6 8
1 3
9 4
2 4
</code></pre>

<h4>output</h4>
<p></p><pre>30
27
48
30
48
</pre><p></p>
<h2>限制与约定</h2>
<p>对于所有数据，满足</p>
<ul>
<li>$1 \le N \le 2\,800$。</li>
<li>$1 \le Q \le 3\,000\,000$。</li>
<li>$1 \le T_i \le 1\,000\,000\,000\ (1 \le i \le N)$。</li>
<li>$1 \le A_i \le 1\,000\,000\,000\ (1 \le i \le N)$。</li>
<li>$1 \le B_i \le 1\,000\,000\,000\ (1 \le i \le N)$。</li>
<li>$1 \le C_i \le 1\,000\,000\,000\ (1 \le i \le N)$。</li>
<li>$A_i \ne B_i\ (1 \le i \le N)$。</li>
<li>$1 \le C_i \le 1\,000\,000\,000\ (1 \le i \le N)$。</li>
<li>$C_i$ 是偶整数 $(1 \le i \le N)$。</li>
<li>$1 \le P_j \le 1\,000\,000\,000\ (1 \le j \le Q)$。</li>
<li>$1 \le X_j \le 1\,000\,000\,000\ (1 \le j \le Q)$。</li>
</ul>
<p>各子任务分值及限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">分值</th>
<th style="text-align:center;">限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$T_i \le 3\,000$，$A_i \le 3\,000$，$B_i \le 3\,000\ (1 \le i \le N)$，$P_j \le 3\,000$，$X_j \le 3\,000\ (1 \le j \le Q)$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$Q=1$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">$Q \le 3\,000$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$Q \le 40\,000$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$52$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p>祝大家一遍 AC，求不虐萌萌哒测评机！</p>
<p><strong>时间限制：$\texttt{25s}$</strong></p>
<p><strong>空间限制：$\texttt{2GB}$</strong></p>
<h2>下载</h2>
<p><a href="./21019/file/attachment.zip">样例数据下载</a></p>
