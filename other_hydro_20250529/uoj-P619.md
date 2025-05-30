<p>在 IOI 公园将要举行 $N$ 个活动。这些活动编号为 $1$ 到 $N$。第 $i \ (1\le i\le N)$ 个活动会在时刻 $L_i+0.1$ 开始，在时刻 $R_i-0.1$ 结束。其中 $L_i,R_i$ 均为整数。</p>
<p>JOI 君会参加其中恰好 $K$ 个活动。活动开始之后禁止入场，活动结束之前禁止离场。我们忽略在参加两个活动时在两个活动场地之间移动的时间。</p>
<p>JOI 君想要参加编号小的活动。更具体地，令 $a_1,\ldots, a_K\ (1\le a_i&lt;\ldots \le a_K\le N)$ 为 JOI 君参加的活动编号，那么序列 $(a_1,\ldots ,a_K)$ 应该是可能的字典序最小的序列。这里，一个序列 $(a_1,\ldots ,a_K)$ 的字典序比另一个序列 $(b_1,\ldots ,b_K)$ 的字典序小，当且仅当存在 $j\ (1\le j\le K)$ 满足对于所有 $1\le \ell \le j-1$ 有 $a_\ell=b_\ell$ 且 $a_j\le b_j$。</p>
<p>给定活动信息和 JOI 君会参加的活动数 $K$，写一个程序判断 JOI 君是否能参加 $K$ 个活动。如果 JOI 君能参加 $K$ 个活动，这个程序也要求出这 $K$ 个活动的编号。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $N, K$。</p>
<p>接下来 $N$ 行，每行两个整数 $L_i,R_i$。</p>
<h2>输出格式</h2>
<p>如果 JOI 君不能参加 $K$ 个活动，输出一行一个整数 <code>-1</code> 到标准输出。</p>
<p>如果 JOI 君可以参加 $K$ 个活动，输出 $K$ 行到标准输出。令 $a_1,\ldots, a_K\ (1\le a_1&lt;\ldots \le a_K\le N)$ 为 JOI 君会参加的活动编号，输出的第 $j\ (1\le j\le K)$ 行应包含 $a_j$。此处 $(a_1,\ldots ,a_K)$ 应该是所有可能的序列中字典序最小的一个。</p>


<pre><code class="language-input1">5 4
1 3
2 5
8 9
6 8
10 15
</code></pre>


<pre><code class="language-output1">1
3
4
5
</code></pre>


<p>JOI 君恰好参加 $4$ 个活动有两种方式：</p>
<ul>
<li>JOI 君会参加活动 $1,3,4,5$；</li>
<li>JOI 君会参加活动 $2,3,4,5$。</li>
</ul>
<p>因为序列 $(1,3,4,5)$ 的字典序比序列 $(2,3,4,5)$ 小，所以输出 $1,3,4,5$。</p>


<pre><code class="language-input2">4 3
1 4
3 5
4 9
7 10
</code></pre>


<pre><code class="language-output2">-1
</code></pre>


<p>因为 JOI 君不可能参加恰好 $3$ 个活动，所以输出 $-1$。</p>
<h2>样例三</h2>
<p>这个样例输入满足所有子任务的限制。</p>

<pre><code class="language-input2">10 6
77412002 93858605
244306432 318243514
280338037 358494212
439397354 492065507
485779890 529132783
571714810 632053254
659767854 709114867
718405631 733610573
786950301 815106357
878719468 899999649
</code></pre>


<pre><code class="language-output2">1
2
4
6
7
8
</code></pre>



<pre><code class="language-input4">20 16
250732298 258217736
26470443 34965880
252620676 260043105
692063405 697656580
497457675 504191511
391372149 397942668
858168758 867389085
235756850 241022021
585764751 593366541
207824318 217052204
661682908 671226688
886273261 892279963
770109416 778960597
264372562 270395107
176883483 186662376
509929119 519063796
109491630 118520141
162731982 168101507
662727316 668317158
757072772 765493222
</code></pre>


<pre><code class="language-output4">1
2
4
5
6
7
8
9
10
11
12
13
14
15
16
17
</code></pre>

<h2>限制与约定</h2>
<p>对于全部数据，满足：</p>
<ul>
<li>$1\le N\le 10^5$</li>
<li>$1\le K\le N$</li>
<li>$1\le L_i\le R_i\le 10^9\ (1\le i\le N)$</li>
</ul>
<p>详细子任务附加限制及分值如下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$L_i\le L_{i+1}\ (1\le i\le N-1)$</td>
<td style="text-align:center;">$7$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$N\le 20$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$N\le 2\ 000$</td>
<td style="text-align:center;">$31$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">无附加限制</td>
<td style="text-align:center;">$61$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{3s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="./21021/file/attachment.zip">样例数据下载</a></p>
