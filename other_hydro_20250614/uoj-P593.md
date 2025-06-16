<p>黑衣人 $04$ 是一个非常可怕的人，他有一支由 $n$ 个人构成的军队 <code>in's army</code>，而这只军队看守着神牪牪。</p>
<p>军队每个人有一个等级，每个人等级互不相同。庚子年即将过去，辛丑年即将到来，原来等级第 $i$ 高的人，新的一年等级会变成第 $p_i$ 高，可以发现 $p$ 是一个排列。</p>
<p>对于原来等级第 $i$ 高的人，若 $p_{i} &gt; p_{i+1}$，即他等级没有原来比他菜的那个人高，他就会不高兴，特别的原来等级最低的人不会不高兴。</p>
<p>你有一个小弟，早早混入了黑衣人 $04$ 的军队，他在过去一年排名为 $k$。并且他打听到不高兴的人（包括他自己）个数为 $m$。</p>
<p>你现在想知道对于 $1\le l\le n$ 的每个 $l$，有多少种可能的排名使得小弟的新一年排名为 $l$，这样可以方便你之后的救援，方案数对 $998244353$ 取模。</p>


<h2>输入格式</h2>
<p>一行三个整数，输入 $n,m,k$。</p>
<h2>输出格式</h2>
<p>输出一行 $n$ 个整数，表示对于 $1\le l\le n$ 的每个 $l$，可能的排名数对 $998244353$ 取模后的结果。</p>


<pre><code class="language-input1">4 2 1
</code></pre>


<pre><code class="language-output1">1 2 4 4
</code></pre>



<pre><code class="language-input2">5 0 2
</code></pre>


<pre><code class="language-output2">0 1 0 0 0
</code></pre>



<pre><code class="language-input3">11 2 4
</code></pre>


<pre><code class="language-output3">14880 14160 12816 11640 11496 12480 13896 15093 15696 15600 14880
</code></pre>


<h2>样例四</h2>
<p>见下载文件中的 <code>ex_army4.in</code> 与 <code>ex_army4.ans</code>，该样例符合子任务 $3$ 的限制。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，保证 $1\le n\le 5\times 10^5; 0\le m\le n-1; 1\le k\le n$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">特殊限制</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$n\le 10$</td>
<td style="text-align:center;">$5$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$n\le 300$</td>
<td style="text-align:center;">$15$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$n\le 3\times 10^3$</td>
<td style="text-align:center;">$15$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">$n\le 10^5$</td>
<td style="text-align:center;">$35$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">$k=1$</td>
<td style="text-align:center;">$15$</td>
</tr><tr><td style="text-align:center;">$6$</td>
<td style="text-align:center;">无特殊限制</td>
<td style="text-align:center;">$15$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$4\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="https://uoj.ac/download.php?type=problem&amp;id=593">样例数据下载</a></p>
