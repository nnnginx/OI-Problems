<p>伏特找到了跳蚤国顶尖的工程师们，请他们设计月球列车的引擎。</p>
<p>工程师们设计出了一款非常特殊的引擎——月千引擎。这个引擎由 $n$ 个部件组成，每个部件有一个功耗参数 $a_i$。</p>
<p>当引擎以 $x$ 的速度行进时，引擎的总功耗为 $\oplus_{i=1}^n (a_i+x)$，即 $(a_1 + x) \oplus (a_2 + x) \oplus \cdots \oplus (a_n + x)$，其中 $\oplus$ 表示异或。</p>
<p>现在伏特设置了 $m$ 种不同的速度，你需要快速算出引擎的功耗。由于伏特的暴脾气，你有可能需要得到每一个速度后立马输出答案。</p>
<h2>输入格式</h2>
<p>第一行三个整数 $n, m, t$，表示引擎部件数，询问数量以及加密参数。</p>
<p>第二行 $n$ 个整数，第 $i$ 个整数 $a_i$ 表示部件的功耗参数。</p>
<p>接下来 $m$ 行，第 $i$ 行输入 $v'_i$，表示第 $i$ 个询问的速度 $v_i=v'_i \oplus \left(t \times \left\lfloor\frac{\mathrm{lastans}}{2^{20}}\right\rfloor\right)$，其中 $\oplus$ 表示异或，$\mathrm{lastans}$ 表示上一个询问的输出（如果没有则为 $0$）。</p>
<h2>输出格式</h2>
<p>输出 $m$ 行，第 $i$ 行一个整数 $w_i$ 表示第 $i$ 次询问的功耗。</p>


<pre><code class="language-input1">2 2 0
1 2
2
3
</code></pre>


<pre><code class="language-output1">7
1
</code></pre>


<p>第一次询问的输出为 $(1+2)\oplus(2+2)=3\oplus 4=7$。</p>
<p>第一次询问的输出为 $(1+3)\oplus(2+3)=4\oplus 5=1$。</p>
<h2>样例二、三</h2>
<p>见附件下载。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1\leq n, m\leq 2.5\times 10^5, t\in \{0, 1\}, 0\leq a_i,v'_i\lt 2^{60}$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n,m\leq$</th>
<th style="text-align:center;">$t=$</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">1</td>
<td style="text-align:center;">$10^3$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$2.5\times 10^5$</td>
<td style="text-align:center;">$0$</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$2.5\times 10^5$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{3s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
