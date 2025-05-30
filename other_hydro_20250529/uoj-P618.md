<p>河狸们居住在 $N$ 个岛上。这些岛从 $1$ 到 $N$ 编号，并通过 $N-1$ 座双向连接的桥连通。这些桥的编号为 $1$ 到 $N-1$。桥 $i$ 连接岛 $A_i$ 和 $B_i$。通过桥可以在任意岛之间穿梭。每个岛上有一只河狸定居。</p>
<p>有时，在某些岛上居住的河狸们要聚集到一个岛上开会。当一场会议的出席者确定了之后，满足以下条件的一个岛就被选为开会地址：</p>
<ul>
<li>参会者为了到达这个岛开会所需要经过桥的数量的总和是最小的。</li>
</ul>
<p>这里，当会议的出席者确定时，每位出席者都会经过最少数量的桥前往开会所在岛。</p>
<p>会议出席者都希望会议的候选岛很多。当一场会议的出席者确定时，这场会议的<strong>期待值</strong>等于满足以上条件的岛的个数。对于每个从 $1$ 到 $N$ 的整数 $j$（包括两端），你想知道当有 $j$ 位河狸参会时，这场会议的最大期待值是多少。</p>
<p>给定这些岛的信息，写一个程序计算对每一个参会河狸数，这场会议的最大期待值是多少。</p>
<h2>输入格式</h2>
<p>第一行一个整数 $N$。</p>
<p>接下来 $N-1$ 行，每行两个整数 $A_i,B_i$，用一个空格隔开。</p>
<h2>输出格式</h2>
<p>输出 $N$ 行。第 $j\ (1\le j\le N)$ 行输出当参会者有 $j$ 位时，最大的期待值是多少。</p>


<pre><code class="language-input1">5
1 2
2 3
4 2
3 5
</code></pre>


<pre><code class="language-output1">1
4
1
2
1
</code></pre>


<p>例如，我们考虑居住在岛 $1$ 和岛 $3$ 的河狸参加的会议。对于每一个岛，他们要经过的桥的数量之和按如下方法计算。</p>
<ul>
<li>如果他们在岛 $1$ 聚集，住在岛 $1$ 的河狸不需要过桥，住在岛 $3$ 的河狸需要经过 $2$ 座桥，总和为 $2$；</li>
<li>如果他们在岛 $2$ 聚集，他们经过桥的数量总和为 $2$；</li>
<li>如果他们在岛 $3$ 聚集，他们经过桥的数量总和为 $2$；</li>
<li>如果他们在岛 $4$ 聚集，他们经过桥的数量总和为 $4$；</li>
<li>如果他们在岛 $5$ 聚集，他们经过桥的数量总和为 $4$；</li>
</ul>
<p>所以候选岛为岛 $1,2,3$。因此，这次会议的期待值为 $3$。</p>


<pre><code class="language-input2">7
1 2
2 3
3 4
4 5
2 6
3 7
</code></pre>


<pre><code class="language-output2">1
5
1
3
1
2
1
</code></pre>

<h2>限制与约定</h2>
<p>对于所有数据，保证：</p>
<ul>
<li>$1\le N\le 2\times 10^5$</li>
<li>$1\le A_i,B_i\le N\ (1\le i\le N-1)$</li>
<li>$A_i\neq B_i\ (1\le i\le N-1)$</li>
<li>保证可以通过桥从一个岛前往任意一个岛</li>
</ul>
<p>详细子任务附加条件及分值如下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">附加条件</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$N\le 16$</td>
<td style="text-align:center;">$4$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$N\le 4\ 000$</td>
<td style="text-align:center;">$16$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">无附加限制</td>
<td style="text-align:center;">$80$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{4s}$</strong></p>
<p><strong>空间限制：$\texttt{256MB}$</strong></p>
<h2>下载</h2>
<p><a href="./21020/file/attachment.zip">样例数据下载</a></p>
