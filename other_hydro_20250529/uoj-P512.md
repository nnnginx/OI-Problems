<p>JOI 国共有 $N$ 个房屋，编号为$1$至$N$。房子按从小到大的顺序排列在一条直线上。每个房屋有恰好一名居民，住在房屋$x$的居民被称为居民$x$。</p>
<p>最近新冠疫情爆发，每个居民都染上了新冠病毒。为了解决这个问题，政府提出了$M$个解决方案，第$i$个解决方案会花费$C_i$元，在第$T_i$天晚上治疗所有编号在$[L_i,R_i]$之间的居民。在治疗后每个居民都在当晚治愈。</p>
<p>病毒的传染方式如下:</p>
<ul><li>若居民$x$在第$i$天早上仍然患有新冠病毒，则第$i$天中午，居民$x-1$(若存在)和居民$x+1$若存在也会感染新冠病毒。</li>
</ul><p>你是JOI王国的高官，你现在需要从$M$个治疗方案中选出若干个执行，使得在所有治疗方案执行结束后，全部居民均被治愈。在可以全部治愈的情况下，你希望花费的金额尽量的小。</p>
<h2>输入格式</h2>
<p>第一行两个数字$N,M$。</p>
<p>接下来$M$行，每行四个正整数$T_i,L_i,R_i,C_i$，表示一个治疗方案。</p>
<h2>输出格式</h2>
<p>若不存在全部治愈的选择方案，输出$-1$。</p>
<p>否则输出一个整数表示最小花费的金额。</p>


<pre><code class="language-input1"><code class="sh_plain">10 5
2 5 10 3
1 1 6 5
5 2 8 3
7 6 10 4
4 1 3 1</code>
</code></pre>

<pre><code class="language-output1"><code class="sh_plain">7</code>
</code></pre>

<p>我们采用如下方案:</p>
<ul><li>第二天晚上执行方案$1$，居民$5,6,7,8,9,10$被治愈。</li>
<li>第三天中午居民 $5$ 被感染。</li>
<li>第四天中午居民 $6$ 被感染。</li>
<li>第四天晚上执行方案$5$，居民$1,2,3$被治愈。</li>
<li>第五天中午居民 $3,7$ 被感染。</li>
<li>第五天晚上执行方案$3$，居民$3,4,5,6,7$被治愈。</li>
</ul><p>该方案花费为$7$,可以证明为最小花费。</p>


<pre><code class="language-input2"><code class="sh_plain">10 5
2 6 10 3
1 1 5 5
5 2 7 3
8 6 10 4
4 1 3 1</code>
</code></pre>

<pre><code class="language-output2"><code class="sh_plain">-1</code>
</code></pre>


<pre><code class="language-input3"><code class="sh_plain">10 5
1 5 10 4
1 1 6 5
1 4 8 3
1 6 10 3
1 1 3 1</code>
</code></pre>

<pre><code class="language-output3"><code class="sh_plain">7</code>
</code></pre>
<h2>数据范围</h2>
<p>子任务1($4$分):$T_i=1$。</p>
<p>子任务2($5$分):$M \le 16$。</p>
<p>子任务3($30$分):$M \le 5000$。</p>
<p>子任务4($61$分):无特殊限制。</p>
<p>对于所有测试数据，满足$1 \le N \le 10^9,1 \le M \le 100000,1 \le T_i,C_i \le 10^9,1 \le L_i \le R_i \le N$。</p>
<p>时间限制:$\texttt{3S}$</p>
<p>空间限制:$\texttt{512MB}$</p>
