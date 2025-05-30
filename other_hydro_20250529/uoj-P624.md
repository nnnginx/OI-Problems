<p>Alice 有 $n$ 张卡牌，第 $i$（$1 \le i \le n$）张卡牌的正面有数字 $a_i$，背面有数字 $b_i$，初始时所有卡牌正面朝上。</p>
<p>现在 Alice 可以将不超过 $m$ 张卡牌翻面，即由正面朝上改为背面朝上。Alice 的目标是让最终朝上的 $n$ 个数字的极差（最大值与最小值的差）尽量小。请你帮 Alice 算一算极差的最小值是多少。</p>
<h2>输入格式</h2>
<p>第一行，两个正整数 $n, m$，代表卡牌张数与至多翻面张数。</p>
<p>第二行，$n$ 个正整数，第 $i$ 个数字表示 $a_i$。</p>
<p>第二行，$n$ 个正整数，第 $i$ 个数字表示 $b_i$。</p>
<p>数据保证卡牌上的 $2n$ 个数字互不相同，且卡牌按照 $a_i$ 升序给出。</p>
<h2>输出格式</h2>
<p>仅一行，一个整数，表示答案。</p>


<pre><code class="language-input1">6 3
8 11 13 14 16 19
10 18 2 3 6 7
</code></pre>


<pre><code class="language-output1">8
</code></pre>


<p>最优方案之一：将第 $1, 5, 6$ 张卡牌翻面，最终朝上的数字依次为 $10, 11, 13, 14, 6, 7$，极差为 $14 - 6 = 8$。</p>
<h2>样例二</h2>
<p>见附加文件中 <code>ex_card2.in</code> 与 <code>ex_card2.ans</code>。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_card3.in</code> 与 <code>ex_card3.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试数据：$3 \le n \le 10^6, 1 \le m \lt n, 1 \le a_i, b_i \le {10}^9$。</p>
<p>每个测试点的具体限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \leq$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 4$</td>
<td style="text-align:center;">$500$</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 6$</td>
<td style="text-align:center;">$5\times 10^5$</td>
<td style="text-align:center;">$m \leq 1000$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$1 \times 10^5$</td>
<td style="text-align:center;" rowspan="4">无</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$4 \times {10}^5$</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">$7 \times {10}^5$</td>
</tr>
<tr>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$1 \times {10}^6$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21025/file/attachment.zip">样例数据下载</a></p>
