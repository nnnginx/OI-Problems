<p>伏特找到了 skip 蚤，希望他负责建造月球车站。然而众所周知，skip 蚤是一只大鸽子。于是他掏出了口袋里的硬币，在桌面上摆成了一排，要伏特和他玩一局游戏，结束后就开始干活。</p>
<p>初始时每枚硬币要么正面朝上，要么背面朝上。游戏会一轮轮进行，如果某一时刻（包括初始时刻）所有硬币都是正面，则游戏立刻结束。</p>
<p>每轮的操作如下：</p>
<ol>
<li><p>取出最左侧的硬币。</p>
</li>
<li><p>如果这枚硬币正面朝上，则由 skip 蚤选择是否翻转，否则由伏特选择是否翻转。</p>
</li>
<li><p>将这枚硬币放到最右边。</p>
</li>
</ol>
<p>伏特已经被铁路建造弄昏了头，于是他决定随机翻转。每次轮到他决定时，他选择翻转的概率为 $p$，选择不翻转的概率为 $1-p$，不同轮之间独立。</p>
<p>skip 蚤是一只非常聪明的鸽子，他通过神秘手段知道了伏特的策略，并且他将以最优策略决定是否翻转来使游戏期望进行轮数尽可能大。</p>
<p>求游戏期望进行几轮，答案对 $998244353$ 取模。</p>
<h2>输入格式</h2>
<p>第一行一个长度为 $n$ 的 <samp>01</samp> 串，表示初始的硬币序列，<samp>0</samp> 表示硬币背面朝上，<samp>1</samp> 表示硬币正面朝上。</p>
<p>第二行两个整数 $a, b$，表示 $p=\frac{a}{a+b}$。</p>
<h2>输出格式</h2>
<p>输出一个整数，表示 skip 蚤在使用最优策略的情况下，游戏结束所需要的期望轮数。</p>
<p>如果游戏轮数的期望不收敛，则输出 $-1$。</p>
<p>否则，题目数据保证了该期望必定可以写成一个分数 $\frac{c}{d}$ ($c \ge 0, d \ge 1$)，且分母 $d$ 不是 $998244353$ 的倍数。请输出一个整数 $x \in [0, 998244353)$ 使得 $dx$ 和 $c$ 在模 $998244353$ 意义下同余。</p>


<pre><code class="language-input1">10
1 1
</code></pre>


<pre><code class="language-output1">8
</code></pre>


<p>当局面为 <samp>10</samp> 时，skip 蚤会选择翻转变为 <samp>00</samp>。</p>
<p>此时伏特有 $\frac 12$ 的概率翻转使局面变为 <samp>01</samp>，$\frac 12$ 的概率不翻转使局面不变，即期望两轮后局面变为 <samp>01</samp>。</p>
<p>接下来伏特有 $\frac 12$ 的概率翻转使游戏结束，$\frac 12$ 的概率不翻转使局面重新变为 <samp>10</samp>。</p>
<p>整体来看，局面为 <samp>10</samp> 时，期望经过四轮后，有$\frac 12$ 的概率游戏结束，$\frac 12$ 的概率局面重新变为 <samp>10</samp>。因此游戏期望进行轮数为 $8$ 轮。</p>


<pre><code class="language-input2">0011
1 0
</code></pre>



<pre><code class="language-output2">2
</code></pre>


<p>由于伏特一定会翻转背面硬币，所以两轮以后所有硬币都正面朝上了。</p>


<pre><code class="language-input3">0101
1 0
</code></pre>


<pre><code class="language-output3">-1
</code></pre>


<p>由于伏特会一直翻转，skip 蚤也只需一直翻转即可保证游戏不会结束。</p>
<h2>样例四</h2>
<p>见附件下载。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1\leq n \leq 23$，$0\leq a, b \leq 998244352, 998244353\nmid a+b$。</p>
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
<td style="text-align:center;">1</td>
<td style="text-align:center;" rowspan="2">$23$</td>
<td style="text-align:center;">$a=0$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">2</td>
<td style="text-align:center;">$b=0$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">3</td>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$a,b\leq 10$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">4</td>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$30$</td>
</tr>
<tr>
<td style="text-align:center;">5</td>
<td style="text-align:center;">$23$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$45$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>后记</h2>
<p>由于 skip 蚤实在是太鸽了，愤怒的跳蚤国王把 skip 蚤抓回去煲成了汤。</p>
