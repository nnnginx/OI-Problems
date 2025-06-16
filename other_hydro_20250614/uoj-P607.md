<p>蛐蛐国幅员辽阔，全国总共有 $n$ 座城市，其中 $1$ 号城市是首都。因为城市数目太多，在城市之前通信就成了一个大难题。</p>
<p>在战争发生之前，科技落后的蛐蛐国还在采用最原始的方式通信——由一些跳得很快的蛐蛐担任邮差，在城市间往返传递信件。因为这些蛐蛐真的跳得很快（比香港记者还要快），所以蛐蛐国还能维持正常的通信。但是在经过了漫长的战争后，全国大部分的道路都受到了严重的破坏。这些跳得很快的蛐蛐，在受到严重破坏的道路上也只能慢慢跳，城市间的通信效率就变得低下了。翻修道路需要花费大量的蛐力财力，在短期内看不到希望。</p>
<p>伏特决定用跳蚤国的高新技术——跳蚤电话来解决这个难题。跳蚤电话是两两成对的，每一对跳蚤电话都可以发出跳蚤波来相互传递信息。很容易知道，最少只需要在 $n-1$ 对城市间安装跳蚤电话，任意两座城市间就都可以直接或间接通话了。</p>
<p>现在伏特已经拟定了一个最终的安装计划，里面包含了要安装跳蚤电话的 $n-1$ 对城市。但现在安装这些电话的顺序却成了一个难题，伏特决定按下面的方式来安装它们：</p>
<ul>
<li>初始时，没有任何城市安装了电话。令当前可以与 $1$ 号城市直接或间接通信的城市集合为 $S$  ，初始时 $S=\{1\} $。</li>
<li>每一轮有两种操作：选择一对在 $S$ 中且当前可以<strong>直接</strong>通信（即有成对电话）的城市 $x$ 和 $y$ （$x &lt; y$），再选择另一个不在 $S$ 中的城市 $z$  ，撤去 $x$ 和 $y$ 间成对的电话，并分别在 $x$ 和 $z$ 及 $y$ 和 $z$ 间设立成对的电话，将 $z$ 加入 $S$ ；或是选择一个在 $S$ 中的城市 $x$ 和不在 $S$ 中的城市 $y$ ，在 $x$ 和 $y$ 间设立成对电话，将 $y$ 加入 $S$ 。</li>
<li>重复上述过程，直到所有城市都在 $S$ 中。显然，恰好会执行 $n-1$ 轮上面的过程。</li>
</ul>
<p>容易看出，上面的安装方式不仅需要进行的操作数目较少，且能保证任意时刻在 $S$ 中的城市都能直接或间接通信。</p>
<p>但容易发现即使给定了最终的安装计划，按上述方式完成计划的具体方案也不是唯一的。伏特决定从所有可能的具体方案中随机一个，于是他要你先计算出可能的方案总数。由于答案可能很大，你只需要输出答案对 $998244353$ 取模后的值。</p>
<p>两个方案是不同的，当且仅当某一轮执行的操作不完全相同。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $n$ 。</p>
<p>接下来 $n-1$ 行，每行两个正整数 $u_i,v_i$ ，表示安装计划中一对安装电话的城市。</p>
<h2>输出格式</h2>
<p>输出一行一个非负整数，表示答案对 $998244353$ 取模后的值。</p>


<pre><code class="language-input1">4
1 2
2 3
2 4
</code></pre>


<pre><code class="language-output1">4
</code></pre>


<p>我们用 $(x,y,z)$ 和 $(x,y)$ 分别表示两种操作，有如下 $4$ 种合法的方案：</p>
<p>方案 $1$ ： $(1,2),(2,3),(2,4)$ 。</p>
<p>方案 $2$ ： $(1,2),(2,4),(2,3)$ 。</p>
<p>方案 $3$ ： $(1,3),(1,3,2),(2,4)$ 。</p>
<p>方案 $4$ ： $(1,4),(1,4,2),(2,3)$ 。</p>


<pre><code class="language-input2">10
1 9
4 8
10 6
9 7
7 3
4 6
5 7
6 3
2 9
</code></pre>


<pre><code class="language-output2">56980
</code></pre>

<h2>样例三</h2>
<p>见附加文件中 <code>ex_telephone3.in</code> 和 <code>ex_telephone3.out</code> 。</p>
<h2>数据范围</h2>
<p>对于所有数据， $2\leq n\leq 10^5,1\leq u_i,v_i \leq n$ ，保证给定的计划是合法的，即任意一对城市都可以直接或间接通信。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="4">无</td>
<td style="text-align:center;">$9$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$11$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$200$</td>
<td style="text-align:center;">$16$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="2">$10^5$</td>
<td style="text-align:center;">从 $1$ 号城市到任意城市的最短通信路径上城市个数不超过 $3$</td>
<td style="text-align:center;">$14$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$29$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21011/file/attachment.zip">样例数据下载</a></p>
