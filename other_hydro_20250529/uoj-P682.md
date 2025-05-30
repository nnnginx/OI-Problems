<p>伏特再次找到了工程师，请他们设计铁轨。工程师很快给出了一张模板图纸作为候选方案。</p>
<p>图纸上 $n$ 段铁轨排成一行，依次编号为 $1, \dots, n$。根据工程师们的设计，第 $i$ 段铁轨的尾部只能和第 $i+1$ 段铁轨的头部相连 $(1\leq i &lt; n)$，否则铁轨会变的极为不稳定。</p>
<p>伏特不必铺设所有的铁轨。伏特可以选择一个编号区间，如 $[l, r]$，然后下令只铺设编号在区间 $[l, r]$ 中的铁轨。显然区间的选择方案一共只有 $\frac{n(n+1)}{2}$ 种。</p>
<p>跳蚤国拥有独特的材料科学，每段铁轨都可以使用两种材料中的一种构建，稳定度分别为 $a_i,b_i$，且不同段铁轨可以使用不同材料。根据工程师们的建模，对于一个区间选择方案 $[l, r]$，如果第 $i$ 段铁轨选择了稳定度为 $p_i$ 的材料 ($p_i \in \{a_i, b_i\}$)，那么铺设区间 $[l, r]$ 中的所有铁轨的总稳定度为该区间内<strong>所有 $p_i$ 的异或和</strong>，即 $p_l \oplus p_{l+1} \oplus \cdots \oplus p_r$，其中 $\oplus$ 表示异或。</p>
<p>对于每个区间 $[l, r]$，工程师早已算好了在所有可能的材料选择方案中总稳定度的最大值，称之为该区间的<strong>最优稳定度</strong>。</p>
<p>现在伏特找到了你，希望你能帮工程师们验算一番。请你求出所有可能的区间中，第 $k$ 小的最优稳定度是多少。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $n, k$，表示铁轨段数和要求的最优稳定度排名。</p>
<p>第二行 $n$ 个整数，第 $i$ 个整数为 $a_i$，表示使用材料一修建的稳定度。</p>
<p>第三行 $n$ 个整数，第 $i$ 个整数为 $b_i$，表示使用材料二修建的稳定度。</p>
<h2>输出格式</h2>
<p>一行一个整数表示第 $k$ 小的最优稳定度。</p>


<pre><code class="language-input1">3 3
1 2 3
4 5 6
</code></pre>


<pre><code class="language-output1">6
</code></pre>


<p>六种区间选择方案对应的最优稳定度分别为</p>
<ul>
<li>区间 $[1,1]$: 最优稳定度为 $4$;</li>
<li>区间 $[1,2]$: 最优稳定度为 $6$;</li>
<li>区间 $[1,3]$: 最优稳定度为 $7$;</li>
<li>区间 $[2,2]$: 最优稳定度为 $5$;</li>
<li>区间 $[2,3]$: 最优稳定度为 $6$;</li>
<li>区间 $[3,3]$: 最优稳定度为 $6$.</li>
</ul>


<pre><code class="language-input2">10 1
3 30 30 20 10 4 24 0 17 16
3 3 14 19 26 28 13 13 2 27
</code></pre>


<pre><code class="language-output2">3
</code></pre>

<h2>样例三、四、五、六</h2>
<p>见附件下载。</p>
<p>样例四，五分别满足特殊性质 A,B</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1\leq n\leq 10^5,1\leq m \leq 30,0\leq a_i,b_i\lt 2^m,1\leq k\leq \frac{n(n+1)}{2}$，其中 $m$ 是用于限定值域的参数。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">$m=$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">$10^3$</td>
<td style="text-align:center;" rowspan="2">$20$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$3\times 10^4$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;" rowspan="4">$10^5$</td>
<td style="text-align:center;" rowspan="4">$30$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">B</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">C</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">6</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$30$</td>
</tr>
</tbody>
</table>
</div>
<p>特殊性质说明：</p>
<ul>
<li>A: $a_i,b_i$ ($1\leq i\leq n$) 均在 $[0,2^m)$ 范围内独立等概率随机。</li>
<li>B: $a_i=b_i$ ($1\leq i\leq n$)。</li>
<li>C: $a_i=0$ ($1\leq i\leq n$)。</li>
</ul>
<p><strong>时间限制：$\texttt{4s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
