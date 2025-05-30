<p>Maryam 是一位电机工程师。她正在为一座通讯塔设计接线方案。在这个塔上有一些分布在不同高度的连接点。一条电线可以用来将任何两个连接点接起来。每一个连接点都可以接上任意数目的电线。而连接点共有两种：分别为红色连接点及蓝色连接点。</p>
<p>为了表述方便起见，通讯塔会被视为一条直线，而那些红色及蓝色连接点会被视为在这条直线上的一些非负整数坐标。一条电线的长度是该电线所连接的两个连接点间的距离。</p>
<p>你要做的是帮 Maryam 找出一个接线的方案，使得满足以下条件：</p>
<ol>
<li>每个连接点上最少有一条电线连接到一个不同颜色的连接点上</li>
<li>所用的电线的总长度为最短。</li>
</ol>
<h2>实现细节</h2>
<p><strong>本题只支持C++。</strong></p>
<p>你需要实现以下的子程序：</p>
<pre><code class="sh_cpp"> long long min_total_length(std::vector&lt;int&gt; r, std::vector&lt;int&gt; b)</code></pre>
<ul>
<li>$r$: 一个长度为 $n$ 的数组，其内以升序排列着所有红色连接点的位置。</li>
<li>$b$: 一个长度为 $m$ 的数组，其内以升序排列着所有蓝色连接点的位置。 </li>
<li>这个子程序需返回在所有可能的连接方案中，最短电线总长度的那个方案的电线总长度作为其返回值。</li>
<li>请注意这个子程序的返回值的类型为 <code>long long</code>。</li>
</ul>
<h2>例子</h2>
<p>评测程序调用了 <code>min_total_length([1, 2, 3, 7], [0, 4, 5, 9, 10])</code>。</p>
<p>以下的图表述了样例中的数据。</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/321/wiring.png" alt="样例解释"></p>
<ul>
<li>图中以水平的方式表示出相关的通讯塔。</li>
<li>因题目打印是黑白色的，所以红色接点以较深色来表示，而蓝色接点以较浅色来表示。</li>
<li>图中有 $4$ 个红色的连接点，其位置分别为 $1,2,3$ 及 $7$。</li>
<li>图中有 $5$ 个蓝色的连接点，其位置分别为 $0,4,5,9$ 及 $10$。</li>
<li>该例的最优解的电线总长度为 $1+2+2+2+3=10$，所以子程序的返回值为 $10$。</li>
<li>注意共有两条电线连接在位置为 $7$ 的连接点上。</li>
</ul>
<h2>数据范围</h2>
<ul>
<li>$1\leq n,m\leq 100\ 000$</li>
<li>$0\leq r[i]\leq 10^9 $（对于所有 $0 \leq i \leq n-1$）</li>
<li>$0\leq b[i]\leq 10^9 $（对于所有 $0 \leq i \leq m-1$）</li>
<li>数组 $r$ 及 $b$ 都已经按升序排好序。</li>
<li>在数组 $r$ 及 $b$ 的所有 $n+m$ 个值均是不同的。</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">限制与约定</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$n,m\leq 200$</td>
<td style="text-align:center;">$7$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">所有红色接点的位置坐标小于任何蓝色接点的位置坐标</td>
<td style="text-align:center;">$13$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">在每 $7$ 个连续（接续）的连接点内必有最少一个红色接点及一个蓝色接点</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">所有接点在 $[1,n+m]$ 范围内有不同的位置坐标</td>
<td style="text-align:center;">$25$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">无附加限制</td>
<td style="text-align:center;">$45$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>评分程序样例</h2>
<p>评分程序样例将会读入以下格式的数据：</p>
<ul>
<li>第 $1$ 行：$n,m$</li>
<li>第 $2$ 行：$r[0]\ r[1]\ ... \ r[n-1]$</li>
<li>第 $3$ 行：$b[0]\ b[1]\ ... \ b[m-1]$</li>
</ul>
<p>评分程序样例将会输出单独一行数据，上面含有 <code>min_total_length</code> 的返回值。</p>
<h2>下载</h2>
<p><a href="./20748/file/attachment.zip">样例数据与样例评测库下载</a></p>
