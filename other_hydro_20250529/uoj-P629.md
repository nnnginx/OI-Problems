<p>封榜是 ICPC 系列竞赛中的一个特色机制。ICPC 竞赛是实时反馈提交结果的程序设计竞赛,参赛选手与场外观众可以通过排行榜实时查看每个参赛队伍的过题数与排名。竞赛的最后一小时会进行“封榜”,即排行榜上将隐藏最后一小时内的提交的结果。赛后通过滚榜环节将最后一小时的结果（即每只队伍最后一小时的过题数）公布。</p>
<p>Alice 围观了一场 ICPC 竞赛的滚榜环节。本次竞赛共有 $n$ 支队伍参赛，队伍从 $1 \sim n$ 编号，$i$ 号队伍在封榜前通过的题数为 $a_i$。排行榜上队伍按照过题数从大到小进行排名，若两支队伍过题数相同，则编号小的队伍排名靠前。滚榜时主办方以 $b_i$ 不降的顺序依次公布了每支队伍在封榜后的过题数 $b_i$ （最终该队伍总过题数为 $a_i + b_i$），并且每公布一支队伍的结果，排行榜上就会实时更新排名。</p>
<p>Alice 并不记得队伍被公布的顺序，也不记得最终排行榜上的排名情况，只记得每次公布后，本次被公布结果的队伍都成为了新排行榜上的第一名，以及所有队伍在封榜后一共通过了 $m$ 道题（即 $\sum_{i=1}^n b_i = m$）。</p>
<p>现在 Alice 想请你帮她算算，最终排行榜上队伍的排名情况可能有多少种。</p>
<h2>输入格式</h2>
<p>第一行包含两个正整数 $n, m$，表示队伍数量与它们封榜后的总过题数。</p>
<p>第二行包含 $n$ 个正整数表示 $a_i$。</p>
<h2>输出格式</h2>
<p>仅一行一个整数表示答案。</p>


<pre><code class="language-input1">3 6
1 2 1
</code></pre>


<pre><code class="language-output1">5
</code></pre>



<pre><code class="language-input2">6 50
4 7 9 3 0 3
</code></pre>


<pre><code class="language-output2">96
</code></pre>


<ol>
<li>最终排名：$1, 3, 2$，滚榜情况（按公布顺序，下同）：$b_2 = 0,b_3 = 2,b_1 = 4$。</li>
<li>最终排名：$2, 1, 3$，滚榜情况：$b_3 = 2,b_1 = 2,b_2 = 2$。</li>
<li>最终排名：$2, 3, 1$，滚榜情况：$b_1 = 1,b_3 = 2,b_2 = 3$。</li>
<li>最终排名：$3, 1, 2$，滚榜情况：$b_2 = 0,b_1 = 2,b_3 = 4$。</li>
<li>最终排名：$3, 2, 1$，滚榜情况：$b_1 = 1,b_2 = 1,b_3 = 4$。</li>
</ol>


<pre><code class="language-input3">11 300
6 8 8 12 0 11 6 1 0 15 5
</code></pre>


<pre><code class="language-output3">30140983
</code></pre>

<h2>限制与约定</h2>
<p>对于所有测试数据：$1 \leq n \leq 13, 1 \leq m \leq 500, 0 \leq a_i \leq 10^4$。</p>
<p>每个测试点的具体限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \leq$</th>
<th style="text-align:center;">$m \leq$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="2">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 5$</td>
<td style="text-align:center;">$3$</td>
</tr>
<tr>
<td style="text-align:center;">$6 \sim 8$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$100$</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 12$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$200$</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 16$</td>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">$300$</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 20$</td>
<td style="text-align:center;">$13$</td>
<td style="text-align:center;">$500$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21030/file/attachment.zip">样例数据下载</a></p>
