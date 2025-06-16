<p>UOI 的题面是一个外星八爪鱼用脚写的。</p>
<p>由于题面写的很差，大D米不得不不断提问来确认题意。但外星八爪鱼没有手回复，只好叫你来帮忙。</p>
<p>这些问题可以抽象成一个栈的结构，初始为空，大D米有两种操作：</p>
<ul>
<li><code>push</code>：新提一个问题置于栈顶。此时你需要对问题做出以下两种回应之一：R（no Response）或 B（Buzhidao）。</li>
<li><code>pop</code>：大D米在胡乱提交后知道了栈顶问题的答案，问题从栈中移除。</li>
</ul>
<p>这些操作按时间顺序形成了一个长为 $2k$ 的操作序列，保证操作序列合法，且做完所有操作后栈中没有元素。</p>
<p>你需要保证任意时刻栈中 R 类回应数量不超过 $c_r$，B 类回应数量不超过 $c_b$，否则会被大D米发现你是随便回的。</p>
<p>两种回应都很敷衍，B 类回应更让人愤怒。如果你的整个回应过程中，做出了 $p_r$ 次 R 类回应，$p_b$ 次 B 类回应，大D米的愤怒值将是 $p_rp_b^2$。</p>
<p>现在，你想知道所有回应方案中大D米愤怒值的总和。答案可能很大，你只需要输出其对 $998244353$ 取模的结果。</p>
<h2>输入格式</h2>
<p>第一行三个整数 $k,c_r,c_b$，表示操作序列长度、栈中 R 类回应数量限制、栈中 B 类回应数量限制。</p>
<p>接下来 $2k$ 行每行一个为 <code>push</code> 或 <code>pop</code> 的字符串，描述操作序列。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，表示所有回应方案中大D米愤怒值的总和对 $998244353$ 取模后的结果。</p>


<pre><code class="language-input1">3 1 2
push
push
push
pop
pop
pop
</code></pre>


<pre><code class="language-output1">12
</code></pre>


<p>由于操作过程是先放入三个问题再依次移除，所以要求三个回复中恰好有 $1$ 个是 R，$2$ 个是 B。总共有 $\binom{3}{2} = 3$ 个方案，每个方案的愤怒值都是 $1 \times 2^2 = 4$，所以答案为 $3 \times 4 = 12$。</p>


<pre><code class="language-input2">3 1 2
push
push
pop
push
pop
pop
</code></pre>


<pre><code class="language-output2">14
</code></pre>


<p>若第一个问题回的是 R，则剩余两个问题都只能选择回 B，总共有 $1$ 种方案，权值为 $1 \times 2^2 = 4$；</p>
<p>若第一个问题回的是 B，则剩余两个问题没有限制。</p>
<ul>
<li>若这两次都回 B，则有 $1$ 种方案，权值为 $0 \times 3^2 = 0$；</li>
<li>若这两次都回 R，则有 $1$ 种方案，权值为 $2 \times 1^2 = 2$；</li>
<li>若这两次回应不同，则有 $2$ 种方案，权值为 $1 \times 2^2 = 4$。</li>
</ul>
<p>所以所有方案的愤怒值和为 $1 \times 4 + 1 \times 0 + 1 \times 2 + 2 \times 4 = 14$。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_stack3.in</code> 与 <code>ex_stack3.out</code>，该组样例满足子任务 1 的性质。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_stack4.in</code> 与 <code>ex_stack4.out</code>，该组样例满足子任务 3 的性质。</p>
<h2>样例五</h2>
<p>见附加文件中 <code>ex_stack5.in</code> 与 <code>ex_stack5.out</code>，该组样例满足子任务 5 的性质。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1 \leq k \leq 2500, 0 \leq c_r,c_b \leq k$，保证操作序列合法，且做完所有操作后栈中没有元素。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$k\le$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;" rowspan="4">无</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$40$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$80$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$250$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">$2500$</td>
<td style="text-align:center;">$c_r = 1$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$c_r=c_b=k$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$15$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{1s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
