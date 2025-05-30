<p><strong>由于某些原因本题仅支持 C++, C++11 语言的提交。</strong></p>
<p>Robert 正在设计一款新的电脑游戏。游戏中有一位英雄、$n$ 个敌人和 $n + 1$ 个地牢。敌人从 $0$ 到 $n - 1$ 编号，地牢从 $0$ 到 $n$ 编号。敌人 $i$（$0 \le i \le n - 1$）处在地牢 $i$，其能力值为 $s[i]$。地牢 $n$ 里没有敌人。</p>
<p>英雄一开始进入地牢 $x$，初始能力值为 $z$。每次英雄进入地牢 $i$（$0 \le i \le n - 1$）时，都需要面对敌人 $i$，且会发生以下情况中的一种：</p>
<ul>
<li><p>如果英雄的能力值大于等于敌人 $i$ 的能力值 $s[i]$，那么英雄会胜出。这使得英雄的能力值<strong>增加</strong> $s[i]$（$s[i] \ge 1$）。这种情况下，下一步英雄将会进入地牢 $w[i]$（$w[i] &gt; i$）。</p>
</li>
<li><p>否则英雄会战败，这使得英雄的能力值<strong>增加</strong> $p[i]$（$p[i] \ge 1$）。在这种情况下，下一步英雄将会进入地牢 $l[i]$。</p>
</li>
</ul>
<p>注意 $p[i]$ 可能会小于、等于、大于 $s[i]$，$l[i]$ 可能会小于、等于、大于 $i$。无论对战结果如何，敌人 $i$ 始终处在地牢 $i$，且能力值为 $s[i]$。</p>
<p>当英雄进入地牢 $n$ 的时候，游戏结束。可以看出无论英雄的起始地牢和初始能力值如何，游戏一定会在有限次对战之后结束。</p>
<p>Robert 希望你通过 $q$ 次模拟来对游戏进行测试。对于每次模拟，Robert 输入英雄的起始地牢 $x$ 和初始能力值 $z$。你需要做的是对于每次模拟给出游戏结束时英雄的能力值。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>keys.h</code> 头文件。</p>
<p>你要实现以下函数：</p>
<pre><code class="sh_cpp">void init(int n, int[] s, int[] p, int[] w, int[] l)</code></pre>
<ul>
<li>$n$：敌人的数量。</li>
<li>$s$、 $p$、 $w$、 $l$：长度为 $n$ 的序列。对于每一个 $i$（$0 \le i \le n - 1$）：<ul>
<li>$s[i]$ 是敌人 $i$ 的能力值，也是击败敌人 $i$ 后英雄增加的能力值。</li>
<li>$p[i]$ 是英雄被敌人 $i$ 击败后增加的能力值。</li>
<li>$w[i]$ 是英雄击败敌人 $i$ 后进入的下一个地牢的编号。</li>
<li>$l[i]$ 是英雄被敌人 $i$ 击败后进入的下一个地牢的编号。</li>
</ul>
</li>
<li>恰好调用此函数一次，且发生在任何对如下的 <code>simulate</code> 函数的调用之前。</li>
</ul>
<pre><code class="sh_cpp">int64 simulate(int x, int z)</code></pre>
<ul>
<li>$x$：英雄的起始地牢编号。</li>
<li>$z$：英雄的初始能力值。</li>
<li>假设英雄的起始地牢编号为 $x$，初始能力值为 $z$，函数的返回值是相应情况下游戏结束时英雄的能力值。</li>
<li>恰好调用此函数 $q$ 次。</li>
</ul>
<h2>输入格式</h2>
<p>评测程序示例以如下格式读取输入数据：</p>
<ul>
<li>第 $1$ 行：$n \; q$</li>
<li>第 $2$ 行：$s[0] \; s[1] \; \ldots \; s[n − 1]$</li>
<li>第 $3$ 行：$p[0] \; p[1] \; \ldots \; p[n − 1]$</li>
<li>第 $4$ 行：$w[0] \; w[1] \; \ldots \; w[n − 1]$</li>
<li>第 $5$ 行：$l[0] \; l[1] \; \ldots \; l[n − 1]$</li>
<li>第 $6 + i$ 行（$0 \le i \le q - 1$）：$x \; z$，是第 $i$ 次调用 <code>simulate</code> 的参数。</li>
</ul>
<h2>输出格式</h2>
<p>评测程序示例以如下格式打印你的答案：</p>
<ul>
<li>第 $1 + i$ 行（$0 \le i \le q - 1$）：第 $i$ 次调用 <code>simulate</code> 的返回值。</li>
</ul>


<pre><code class="language-input1">3 2
2 6 9
3 1 2
2 2 3
1 0 1
0 1
2 3
</code></pre>


<pre><code class="language-output1">24
25
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">init(3, [2, 6, 9], [3, 1, 2], [2, 2, 3], [1, 0, 1])</code></pre>
<p><img src="https://loj-img.upyun.menci.memset0.cn/2021/06/28/60d8a1ab5aa8b.png" alt="" class="img-responsive center-block"></p>
<p>上图对应这次的 <code>init</code> 调用。每一个正方形都代表了一个地牢。对于所有存在敌人的地牢，$s[i]$、$p[i]$ 对应的值都已经在正方形内表示出来了。红色箭头展示了英雄战胜敌人后游戏状态的变化，黑色箭头展示了英雄战败后游戏状态的变化。</p>
<p>这时如果调用 <code>simulate(0, 1)</code>，游戏会以如下方式进行：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">地牢编号</th>
<th style="text-align:center;">英雄在战斗前的能力值</th>
<th style="text-align:center;">胜负结果</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$0$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">战败</td>
</tr>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">战败 </td>
</tr>
<tr>
<td style="text-align:center;">$0$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">胜出</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">战败</td>
</tr>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">胜出</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$15$</td>
<td style="text-align:center;">胜出 </td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$24$</td>
<td style="text-align:center;">游戏结束</td>
</tr>
</tbody>
</table>
</div>
<p>因此，<code>simulate(0, 1)</code> 的返回值应该是 $24$。</p>
<p>这时如果调用 <code>simulate(2, 3)</code>，游戏会以如下方式进行：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">地牢编号</th>
<th style="text-align:center;">英雄在战斗前的能力值</th>
<th style="text-align:center;">胜负结果</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">战败</td>
</tr>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">战败 </td>
</tr>
<tr>
<td style="text-align:center;">$0$</td>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">胜出</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">战败</td>
</tr>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">胜出</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">胜出 </td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$25$</td>
<td style="text-align:center;">游戏结束</td>
</tr>
</tbody>
</table>
</div>
<p>因此，<code>simulate(2, 3)</code> 的返回值应该是 $25$。</p>
<h2>数据范围</h2>
<p>对于所有数据：</p>
<ul>
<li>$1 \le n \le 400 \, 000$</li>
<li>$1 \le q \le 50 \, 000$</li>
<li>$1 \le s[i], p[i] \le {10}^7$（对于所有的 $0 \le i \le n - 1$）</li>
<li>$0 \le l[i], w[i] \le n$（对于所有的 $0 \le i \le n - 1$）</li>
<li>$w[i] &gt; i$（对于所有的 $0 \le i \le n - 1$）</li>
<li>$0 \le x \le n - 1$</li>
<li>$1 \le z \le {10}^7$</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务</th>
<th style="text-align:center;">分值</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$11$</td>
<td style="text-align:center;">$n \le 50 \, 000$，$q \le 100$，$s[i], p[i] \le 10 \, 000$（对于所有的 $0 \le i \le n - 1$）</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$26$</td>
<td style="text-align:center;">$s[i] = p[i]$（对于所有的 $0 \le i \le n - 1$）</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$13$</td>
<td style="text-align:center;">$n \le 50 \, 000$，所有的敌人拥有相同的能力值，即 $s[i] = s[j]$，对于所有的 $0 \le i, j \le n - 1$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$12$</td>
<td style="text-align:center;">$n \le 50 \, 000$，所有的 $s[i]$ 至多有 $5$ 种不同的数值</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$27$</td>
<td style="text-align:center;">$n \le 50 \, 000$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$11$</td>
<td style="text-align:center;">没有额外的约束条件</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{4s}$</strong></p>
<p><strong>空间限制：$\texttt{2GB}$</strong></p>
