<p>你化装为黑衣人侍卫，来到了黑衣人 $01$ 的老巢，神牛就被关押在这里。经过不停的打探，你了解到黑衣人 $01$ 平时的饮食习惯。</p>
<p>最近共有 $n$ 个米其林精品即将出炉，第 $i$ 个米其林精品的特定销售时间为第 $a_i$ 天到第 $b_i$ 天。销售期间，黑衣人 $01$ 可以在米其林餐厅吃这个米其林精品，在第 $b_i$ 天之后，黑衣人 $01$ 就可以在跳蚤餐厅吃这个米其林精品，但不能在米其林餐厅吃到。</p>
<p>黑衣人 $01$ 的食力有限，他每天最多只能吃 $m$ 个米其林精品（包括在米其林餐厅和在跳蚤餐厅）；尽管如此，他还是打算将这 $n$ 个米其林精品吃光。由于黑衣人 $01$ 有着超光速飞车 <code>vf's car</code>，所以它不必在意如何到达地点，只需要吃。</p>
<p>然而，不能如期吃到最新的米其林精品会使黑衣人 $01$ 沮丧，因此，如果黑衣人 $01$ 在第 $c_i$ 天吃了第 $i$ 个米其林精品，且 $c_i &gt; b_i$，则会产生 $c_i - b_i$ 的沮丧值（若 $c_i ≤ b_i$，则沮丧值为 $0$）。</p>
<p>你需要制定一个饮食方案，使所有米其林精品产生的沮丧值的最大值最小，否则，黑衣人 $01$ 将会吃掉神牛。所以，你需要求出这个最小值为多少。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n,m$，表示米其林精品总数和黑衣人 $01$ 每天最多能吃的米其林精品数。</p>
<p>下面 $n$ 行每行两个正整数 $a_i,b_i$，表示每个米其林精品的特定销售时间。</p>
<h2>输出格式</h2>
<p>一个整数，表示最优方案下所有米其林精品产生的沮丧值的最大值的最小值。</p>


<pre><code class="language-input1">10 1
2 3
3 3
4 5
7 8
6 6
3 3
8 10
5 5
1 3
3 4
</code></pre>


<pre><code class="language-output1">2
</code></pre>

<h2>样例二</h2>
<p>见下载文件中的 <code>ex_diet2.in</code> 与 <code>ex_diet2.out</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试点，保证 $1 \le m \le n \le 10^6, 1 \le a_i \le b_i \le 10^9$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n \le $</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$20$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$20$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$50000$</td>
<td style="text-align:center;">$25$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">$10^6$</td>
<td style="text-align:center;">$35$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20994/file/attachment.zip">样例数据下载</a></p>
