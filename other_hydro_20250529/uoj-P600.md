<p>在一个神秘的 OJ 上，小 C 曾经参加过 $n$ 场比赛，其中第 $i(i=1,2,\ldots,n)$ 场比赛获得了 $a_i$ 积分；积分可能是正的，可能是负的，但它一定是一个 $[-2, 2]$ 中的整数。</p>
<p>由于一些原因，小 C 会挑出一个区间的比赛 $[l, r]$，并和大家说：“要是我只打这个区间的比赛，那么我就有 $\sum_{i=l}^r a_i$ 分了！”当然，小 C 会挑选出至少一场比赛，而且选出区间的比赛积分总和是所有区间里最大的，而这个积分总和则是他对自己发挥的满意程度。</p>
<p>随着时间的流逝，小 C 逐渐忘记了自己每场比赛的分数，也忘了他对这些比赛的满意程度，他只记得每种分数的比赛打了多少场，而小 C 想知道，他满意程度最小可能是多少。于是他来请求于你。</p>
<h2>输入格式</h2>
<p><strong>本题有多组测试数据。</strong></p>
<p>第一行一个正整数 $T$，表示数据组数。</p>
<p>下面 $T$ 行，每行 $c_{-2},c_{-1},c_0,c_1,c_2$ 五个非负整数，分别表示每种分数的比赛场数。你可以自行算出 $n=c_{-2}+c_{-1}+c_0+c_1+c_2$。</p>
<h2>输出格式</h2>
<p>每组测试数据输出两行。第一行一个整数，表示小 C 满意程度的可能最小值。</p>
<p>第二行 $n$ 个整数 $a_1,a_2,\ldots,a_n$，表示达到此最小值的<strong>任意一种</strong>可能的比赛得分情况。</p>


<pre><code class="language-inputundefined">1
1 1 0 2 2
</code></pre>


<pre><code class="language-outputundefined">3
1 -1 2 -2 1 2
</code></pre>

<h2>限制与约定</h2>
<p>令 $\sum n$ 表示一组数据中 $n$ 的总和。对所有数据，保证 $1 \le T \le 10000,1 \le n,\sum n \le 5 \times 10^5$。</p>
<table class="table table-bordered table-text-center table-vertical-middle">
<thead><tr><th>子任务编号</th><th>$n \leq $</th><th>特殊性质</th><th>分值</th></tr></thead>
<tbody>
<tr><td>$1$</td><td>$20$</td><td>$T \le 5$</td><td>$18$</td></tr>
<tr><td>$2$</td><td>$40$</td><td>$T \le 5$</td><td>$18$</td></tr>
<tr><td>$3$</td><td>$5 \times 10^5$</td><td>$c_{-2}=0$</td><td>$18$</td></tr>
<tr><td>$4$</td><td>$5 \times 10^5$</td><td>$c_2=0$</td><td>$18$</td></tr>
<tr><td>$5$</td><td>$5 \times 10^5$</td><td>无</td><td>$28$</td></tr>
</tbody></table>

<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21004/file/attachment.zip">样例数据下载</a></p>
