<p>小 C 喜欢跑步，并且非常喜欢在微信步数排行榜上刷榜，为此他制定了一个刷微信步数的计划。</p>
<p>他来到了一处空旷的场地，处于该场地中的人可以用 $k$ 维整数坐标 $(a_1, a_2, \ldots , a_k)$ 来表示其位置。场地有大小限制，第 $i$ 维的大小为 $w_i$，因此处于场地中的人其坐标应满足 $1 \le a_i \le w_i（1 \le i \le k）$。</p>
<p>小 C 打算在接下来的 $P = w_1 \times w_2 \times \ldots \times w_k$ 天中，每天从场地中一个新的位置出发，开始他的刷步数计划（话句话说，他将会从场地中每个位置都出发一次进行计划）。
他的计划非常简单，每天按照事先规定好的路线行进，每天的路线由 $n$ 步移动构成，每一步可以用 $c_i$ 与 $d_i$ 表示：若他当前位于 $(a_1, a_2, \ldots , a_{c_i}, \ldots  , a_k)$，则这一步他将会走到 $(a_1, a_2, \ldots , a_{c_i} + d_i, \ldots  , a_k)$，其中 $1 \le c_i \le k$，$d_i \in \{−1, 1\}$。小 C 将会不断重复这个路线，直到他走出了场地的范围才结束一天的计划。（即走完第 $n$ 步后，若小 C 还在场内，他将回到第 $1$ 步从头再走一遍）。</p>
<p>小 C 对自己的速度非常有自信，所以他并不在意具体耗费的时间，他只想知道 $P$ 天之后，他一共刷出了多少步微信步数。请你帮他算一算。</p>
<h2>输入格式</h2>
<p>第一行两个用单个空格分隔的整数 $n$，$k$。分别表示路线步数与场地维数。</p>
<p>接下来一行 $k$ 个用单个空格分隔的整数 $w_i$，表示场地大小。</p>
<p>接下来 $n$ 行每行两个用单个空格分隔的整数 $c_i$，$d_i$，依次表示每一步的方向，具体意义见题目描述。</p>
<h2>输出格式</h2>
<p>仅一行一个整数表示答案。答案可能很大，你只需要输出其对 $10^9 + 7$ 取模后的值。</p>
<p>若小 C 的计划会使得他在某一天在场地中永远走不出来，则输出一行一个整数 $-1$。</p>


<pre><code class="language-input1">3 2
3 3
1 1
2 -1
1 1
</code></pre>


<pre><code class="language-output1">21
</code></pre>

<h2>样例解释一</h2>
<p>从 $(1, 1)$ 出发将走 $2$ 步，从 $(1, 2)$ 出发将走 $4$ 步，从 $(1, 3)$ 出发将走 $4$ 步。  </p>
<p>从 $(2, 1)$ 出发将走 $2$ 步，从 $(2, 2)$ 出发将走 $3$ 步，从 $(2, 3)$ 出发将走 $3$ 步。  </p>
<p>从 $(3, 1)$ 出发将走 $1$ 步，从 $(3, 2)$ 出发将走 $1$ 步，从 $(3, 3)$ 出发将走 $1$ 步。  </p>
<p>共计 $21$ 步。  </p>


<pre><code class="language-input2">5 4
6 8 6 5
3 1
2 1
1 1
2 1
2 -1
</code></pre>


<pre><code class="language-output2">10265
</code></pre>

<h2>样例三</h2>
<p>见附加文件中的 <code>ex_walk3.in/ans</code>。</p>
<h2>样例四</h2>
<p>见附加文件中的 <code>ex_walk4.in/ans</code>。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \le$</th>
<th style="text-align:center;">$k \le$</th>
<th style="text-align:center;">$w_i \le$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 3$</td>
<td style="text-align:center;">$5$   </td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$3$</td>
</tr>
<tr>
<td style="text-align:center;">$4 \sim 6$</td>
<td style="text-align:center;">$100$</td>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 8$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10^5$</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 12$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$10^6$</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 16$</td>
<td style="text-align:center;">$5 \times 10^5$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$10^6$</td>
</tr>
<tr>
<td style="text-align:center;">$17 \sim 20$</td>
<td style="text-align:center;">$5 \times 10^5$</td>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$10^9$</td>
</tr>
</tbody>
</table>
</div>
<p>对于所有测试点，保证 $1 \le n \le 5 \times 10^5，1 \le k \le 10，1 \le w_i \le 10^9，d_i \in \{−1, 1\}$。</p>
<p><strong>时间限制：$\texttt{1s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="./20987/file/attachment.zip">附加文件下载</a></p>
