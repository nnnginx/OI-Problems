<p>Bitaro 是一位报道程序设计竞赛的专业记者。几天后会举办一次国际程序设计竞赛。Bitaro 准备写一篇文章报道此事。</p>
<p>这次竞赛会有 $N$ 名选手参加，他们从 $1$ 到 $N$ 编号。每名选手都有一个 <strong>rating</strong> 表明他们在程序设计竞赛中的能力。rating 是一个在 $1$ 和 $10^9$ 之间的整数（包括两端）。</p>
<p>Bitaro 已经采访了选手们。他获得了如下信息。</p>
<ul>
<li>选手 $i\ (1\le i\le N)$ 的 rating 大于等于选手 $A_i$。这里可能会出现 $A_i=i$ 的情况。</li>
</ul>
<p>在采访后。Bitaro 从管理 rating 系统的公司处获得了选手的 rating 列表。列表中写有如下信息。</p>
<ul>
<li>选手 $i\ (1\le i\le N)$ 的 rating 等于 $H_i$。</li>
</ul>
<p>Bitaro 试图基于以上信息写一篇报道。然而，rating 列表里选手的 rating 数据可能是有错误的。</p>
<p>因为截稿日马上就要到了，Bitaro 已经没有时间去获取正确的 rating 列表了。因此，Bitaro 决定更改列表中某些选手的 rating 数据，使得列表里的 rating 不会与采访中得到的信息矛盾。更改列表中选手 $i\ (1\le i\le N)$ 的 rating 的花费为 $C_i$。也就是说，Bitaro 可以在花费 $C_i$ 的代价下，将列表中选手 $i$ 的 rating 更改为 $1$ 到 $10^9$ 之间的任意整数（包括两端）。为了赶上截稿日，Bitaro 想要最小化更改 rating 的总花费。</p>
<p>给定选手数，采访中获得的信息，rating 列表和更改每个选手 rating 的花费。写一个程序计算使得 rating 列表不与采访获得信息矛盾的情况下，更改 rating 的最小总花费。</p>
<h2>输入格式</h2>
<p>第一行一个整数 $N$。</p>
<p>接下来 $N$ 行，每行三个整数 $A_i,H_i,C_i$。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，表示最小总花费。</p>


<pre><code class="language-input1">6
1 6 5
1 3 6
1 8 4
3 4 9
2 2 5
2 5 6
</code></pre>


<pre><code class="language-output1">14
</code></pre>


<p>如果 Bitaro 按如下方法更改选手的 rating，那么得到的列表就不会与采访中得到的信息矛盾了。</p>
<ul>
<li>将选手 $1$ 的 rating 由 $6$ 改为 $1$，花费为 $5$。</li>
<li>将选手 $3$ 的 rating 由 $8$ 改为 $4$，花费为 $4$。</li>
<li>将选手 $5$ 的 rating 由 $2$ 改为 $10^9$，花费为 $5$。</li>
</ul>
<p>总花费为 $5+4+5=14$。因为这是最小的总花费，所以输出 $14$。</p>
<p>这组样例满足子任务 $1,2,3$ 的限制。</p>


<pre><code class="language-input2">5
1 1 1
2 2 1
4 3 1
3 3 1
4 3 1
</code></pre>


<pre><code class="language-output2">0
</code></pre>


<p>在这组样例中，列表中选手的 rating 与采访中获得的信息不矛盾，因此最小总花费为 $0$，输出 $0$。</p>
<h2>样例三</h2>
<p>这组样例满足子任务 $1,2,3$ 的限制。</p>

<pre><code class="language-input2">20
1 7 381792936
1 89 964898447
1 27 797240712
3 4 299745243
2 18 113181438
2 20 952129455
4 34 124298446
4 89 33466733
7 40 109601410
5 81 902931267
2 4 669879699
8 23 785166502
8 1 601717183
8 26 747624379
1 17 504589209
9 24 909134233
16 56 236448090
8 94 605526613
5 90 481898834
9 34 183442771
</code></pre>


<pre><code class="language-output2">2711043927
</code></pre>



<pre><code class="language-input4">20
15 62 418848971
13 5 277275513
14 60 80376452
12 14 256845164
12 42 481331310
6 86 290168639
3 98 947342135
3 19 896070909
16 39 48034188
8 29 925729089
18 97 420006994
13 51 454182928
19 61 822405612
13 37 148425187
15 77 474094143
14 27 272926693
18 43 566552069
9 93 790433300
10 73 61654171
14 28 334498030
</code></pre>


<pre><code class="language-output4">4012295156
</code></pre>

<h2>限制与约定</h2>
<p>对于全部数据，满足：</p>
<ul>
<li>$2\le N\le 2\times 10^5$</li>
<li>$1\le A_i\le N\ (1\le i\le N)$</li>
<li>$1\le H_i,C_i\le 10^9\ (1\le i\le N)$</li>
</ul>
<p>详细子任务附加限制及分值如下表所示：</p>
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
<td style="text-align:center;">$N\le 5\ 000,\ A_1=1,\ A_i\le i-1\ (2\le i\le N)$</td>
<td style="text-align:center;">$14$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$A_1=1,\ A_i\le i-1\ (2\le i\le N)$</td>
<td style="text-align:center;">$65$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">无附加限制</td>
<td style="text-align:center;">$21$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="./21022/file/attachment.zip">样例数据下载</a></p>
