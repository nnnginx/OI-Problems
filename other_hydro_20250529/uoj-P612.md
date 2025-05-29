<p>IOI 中心是一个配备了生活设施的训练中心。这里有着为大型团体设置的饮食区。在饮食区内，依次排列着 $N$ 家商店，从 $1$ 到 $N$ 标号。在每家商店前，都有一个为顾客准备的队列。顾客们会在每个队列中排队。</p>
<p>今天有 $M$ 个团体呆在 IOI 中心，从 $1$ 到 $M$ 标号。团体中的成员们会以一种相对奇怪的方式排队，以享受他们之间的闲谈。</p>
<p>在这个饮食区中，有时商店会给予在他们的队列中的顾客免费的甜点。在饮食区中工作的 JOI 君的工作内容是记录被给予免费甜点的顾客所在的团体编号。</p>
<p>没有顾客会在关门的商店前排队。今天，当所有商店都营业时，在队列中发生了 $Q$ 次事件。第 $i$ 次事件是下列几种之一：</p>
<ol>
<li><strong>加入</strong>：对于编号在 $L_i$ 到 $R_i$ 之间（包括边界）的所有商店，来自 $C_i$ 团体的 $K_i$ 位顾客加入于队列的末尾。</li>
<li><strong>离开</strong>：对于编号在 $L_i$ 到 $R_i$ 之间（包括边界）的所有商店，如果队列中有 $K_i$ 或更多位顾客，于队列开头的前 $K_i$ 位顾客离开队列。否则，所有顾客离开队列。</li>
<li><strong>服务</strong>：如果在商店 $A_i$ 前的队列中有 $B_i$ 或更多位顾客，商店会给予队列中从开头数起第 $B_i$ 位顾客一个免费甜点。否则商店的工作人员会吃掉免费甜点。</li>
</ol>
<p>不幸的是，JOI 君丢失了被给予免费甜点的顾客所在的团体编号的记录。他决定利用上述 $Q$ 次事件的信息恢复记录。</p>
<p>给出商店、团体、事件的数量，以及事件的详细信息，请编写一个程序确定每次“服务”时是否有顾客被给予了免费甜点。如果有顾客被给予了免费甜点，程序还应该确定这位顾客所在的团体的编号。</p>
<h2>输入格式</h2>
<p>第一行，三个正整数 $N, M, Q$。</p>
<p>接下来 $Q$ 行，第 $i$ 行描述一个事件：  </p>
<p>令 $T_i$ 为第一个数，则第 $i$ 个询问：</p>
<ol>
<li>如果 $T_i = 1$，同一行接下来四个正整数 $L_i, R_i, C_i, K_i$。表示第 $i$ 次事件为“加入”，并且对于编号在 $L_i$ 到 $R_i$ 之间（包括边界）的所有商店，来自 $C_i$ 团体的 $K_i$ 位顾客加入于队列的末尾。</li>
<li>如果 $T_i = 2$，同一行接下来三个正整数 $L_i, R_i, K_i$。表示第 $i$ 次事件为“离开”，并且对于编号在 $L_i$ 到 $R_i$ 之间（包括边界）的所有商店，如果队列中有 $K_i$ 或更多位顾客，于队列开头的前 $K_i$ 位顾客离开队列。否则，所有顾客离开队列。</li>
<li>如果 $T_i = 3$，同一行接下来两个正整数 $A_i, B_i$。表示第 $i$ 次事件为“服务”，并且如果在商店 $A_i$ 前的队列中有 $B_i$ 或更多位顾客，商店会给予队列中从开头数起第 $B_i$ 位顾客一个免费甜点。否则商店的工作人员会吃掉免费甜点。</li>
</ol>
<h2>输出格式</h2>
<p>对于每次“服务”事件，也就是所有满足 $T_i = 3$ 的事件 $i$（$1 \le i \le Q$）输出一行。如果在第 $i$ 次事件中有顾客被给予了免费甜点，输出这位顾客所在的团体的编号。如果在第 $i$ 次事件中商店的工作人员吃掉了免费甜点，输出 <code>0</code>。</p>


<pre><code class="language-input1">3 5 7
1 2 3 5 2
1 1 2 2 4
3 2 3
2 1 3 3
3 1 2
1 2 3 4 2
3 3 2
</code></pre>


<pre><code class="language-output1">2
0
4
</code></pre>


<p>下面我们用顾客所在团体的整数序列表示队列。例如，如果有 3 个顾客在商店前的队列，而且他们从队头开始分别属于团体 1, 2, 2，我们就写作 $(1,2,2)$。空队列写成 $()$。</p>
<p>在样例输入中，7 个事件发生了。</p>
<ol>
<li>第一个事件是<strong>加入</strong>。2 个团体 5 的顾客加入了商店 2, 3 前的队列，之后商店 1, 2, 3 的队列变成 $(),(5,5),(5,5)$。</li>
<li>第二个事件是<strong>加入</strong>。4 个团体 2 的顾客加入了商店 1, 2 前的队列，之后商店 1, 2, 3 的队列变成 $(2,2,2,2),(5,5,2,2,2,2),(5,5)$。</li>
<li>第三个事件是<strong>服务</strong>。商店 2 有 6 个顾客排队。由于 6 不小于 3，第三个顾客获得了一份免费甜点。第三个顾客属于团体 2，所以输出 <code>2</code>.</li>
<li>第四个时间是<strong>离开</strong>。商店 1, 2 均有至少 3 个顾客排队，因此分别有 3 个顾客离开了。由于商店 3 的队伍不到 3 个顾客，所有顾客均离开。之后商店 1, 2, 3 的队列变成 $(2),(2,2,2),()$。</li>
<li>第五个事件是<strong>服务</strong>。商店 1 只有 1 个顾客排队，1 比 2 小，商店职员会把免费甜点吃掉，因此输出 <code>0</code>。</li>
<li>第六个事件是<strong>加入</strong>。2 个团体 4 的顾客加入了商店 2, 3，之后商店 1, 2, 3 的队列变成 $(2),(2,2,2,4,4),(4,4)$。</li>
<li>第七个事件是<strong>服务</strong>。商店 3 有 2 个顾客排队，因此第二个顾客获得了一份免费甜点。第二个顾客属于团体 4，所以输出 <code>4</code>。</li>
</ol>
<p>此样例满足子任务 $2, 7, 8$ 的限制。</p>


<pre><code class="language-input2">3 4 7
1 1 2 1 1
1 1 3 4 1
2 2 3 1
2 1 3 1
1 1 2 2 1
3 1 1
3 3 2
</code></pre>


<pre><code class="language-output2">4
0
</code></pre>


<p>此样例满足子任务 $1, 2, 3, 5, 7, 8$ 的限制。</p>


<pre><code class="language-input3">183326 218318 22
1 106761 160918 151683 574906362
3 68709 1
1 29240 156379 22166 957318472
1 14054 181502 82845 97183925
2 112033 122908 587808357
2 57819 160939 215041262
3 36674 524274467
1 35854 69866 32334 322730299
1 1384 7230 115069 454256926
1 44192 158235 8750 84192710
3 54457 1077490708
2 10592 110384 979714505
2 44594 79244 311724477
3 160965 97183926
1 88748 101697 39148 373927458
3 41166 58039001
1 91501 137591 205480 958877326
2 77775 169655 135756956
1 12497 57047 60918 15666764
1 47839 51716 144688 732270998
3 114514 774994894
3 48645 169986425
</code></pre>


<pre><code class="language-output3">0
22166
32334
0
82845
8750
60918
</code></pre>

<h2>限制与约定</h2>
<p><strong>本题采用捆绑测试。</strong></p>
<p>对于 $100 \%$ 的数据，$1 \le N, M, Q \le 2.5 \times {10}^5$，$T_i \in \{ 1, 2, 3 \}$，$1 \le L_i, R_i, A_i \le N$，$L_i \le R_i$，$1 \le C_i \le M$，$1 \le K_i \le {10}^9$，$1 \le B_i \le {10}^{15}$，至少存在一次满足 $T_i = 3$ 的事件。</p>
<p>每个子任务的具体限制见下表：</p>
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
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$N, Q \le 2000$，$K_i = 1$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$N, Q \le 2000$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$N, Q \le 65000$，当 $T_i = 1$ 时保证 $R_i - L_i \le 10$ 且 $K_i = 1$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$21$</td>
<td style="text-align:center;">$M = 1$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">$N, Q \le 65000$，$K_i = 1$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$13$</td>
<td style="text-align:center;">$N, Q \le 65000$，$T_i \in \{ 1, 3 \}$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$26$</td>
<td style="text-align:center;">$N, Q \le 65000$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$11$</td>
<td style="text-align:center;">无特殊限制</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{1s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="./21016/file/attachment.zip">样例数据下载</a></p>
