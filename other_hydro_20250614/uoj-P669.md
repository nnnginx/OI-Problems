<p>UOI 的规矩是一些成熟稳重的外星大象制定的，所以大D米 AK 了也不准离场。</p>
<p>无聊的大D米决定预测一下排名。他对 $n$ 名参赛选手的水平进行了建模，形成了一棵大小为 $n$ 的有根树 $T$，根为 $1$，表示大D米自己。设节点 $x$ 的父亲为 $\mathrm{fa}[x]$，保证 $\mathrm{fa}[x] &lt; x$。</p>
<p>根据大D米的建模，$\mathrm{fa}[x]$ 的水平是严格比 $x$ 高的，排名应该在他前面。其他人的排名没那么好确定，但是这棵树上同一个子树的人思维方式很接近，排名连续比较合理。</p>
<p>形式化地，对树 $T$，我们这样定义一个 <code>ddm</code> 过程，用于确定选手的可能排名：</p>
<ul>
<li>令当前已经考虑的节点集合为 $M$，当前正在考虑的节点为 $x$。初始时 $M=\{x\}$ 且 $x=1$。</li>
<li>重复如下过程直到所有节点都在 $M$ 中：<ul>
<li>若 $x$ 的所有儿子均在 $M$ 中，则将 $x$ 改为 $\mathrm{fa}[x]$；</li>
<li>否则，任选一个 $x$ 未被加入 $M$ 中的儿子 $u$，将 $u$ 加入 $M$ 并将 $x$ 改为 $u$。</li>
</ul>
</li>
</ul>
<p>每个 <code>ddm</code> 过程都会对应一个 <code>ddm</code> 序，一个 <code>ddm</code> 序是一个 $1\sim n$ 的排列 $p$，其中 $p_i$ 表示在对应的 <code>ddm</code> 过程中，节点 $i$ 是第 $p_i$ 个加入 $M$ 的。显然，对于树 $T$，可能会有很多不同的 <code>ddm</code> 过程，自然也对应很多不同的 <code>ddm</code> 序。</p>
<p>考完后，大D米发现真实的排名表是一个 $1\sim n$ 的排列 $a$。根据大D米的分析，这是由于考试的随机性保证的。为了圆回去，你需要找到这棵树的一个合法 <code>ddm</code> 序 $p$，使得 $a$ 能通过以下方式生成：</p>
<ul>
<li>初始令 $b=p$。</li>
<li>进行任意次操作直到 $b=a$：<ul>
<li>任选 $x\ne 1$ ，使得 $b[\mathrm{fa}[x]] &lt; b[x]$，然后交换 $b[\mathrm{fa}[x]]$ 和 $b[x]$。</li>
</ul>
</li>
</ul>
<p>对于某些排列 $a$，可能会出现没有合法 <code>ddm</code> 序的情况，这时候你需要报告无解。</p>
<h2>输入格式</h2>
<p>第一行一个整数 $tp$，表示测试点所在的测试包编号。</p>
<p>第二行一个整数 $n$，表示树 $T$ 的点数。</p>
<p>第三行 $n$ 个整数，第 $i$ 个整数表示 $a_i$。</p>
<p>第四行 $n-1$ 个整数，第 $i$ 个整数表示 $\mathrm{fa}[i+1]$ ，即 $i+1$ 的父亲。</p>
<h2>输出格式</h2>
<p>如果存在合法的 <code>ddm</code> 序 $p$，输出一行 $n$ 个整数，第 $i$ 个整数表示 $p_i$（即节点 $i$ 在对应 <code>ddm</code> 过程中是第 $p_i$ 个加入 $M$ 的）。如果有多个合法的 $p$，你可以任意输出一个。</p>
<p>否则，你只需要输出一行 <code>-1</code>。</p>


<pre><code class="language-input1">1
5
5 3 1 2 4
1 2 2 1
</code></pre>


<pre><code class="language-output1">1 2 3 4 5
</code></pre>


<p>记交换 $b[\mathrm{fa}[x]],b[x]$ 的操作为 <code>swap(fa[x],x)</code>。</p>
<p>一种可行的构造 $a$ 的方案是： <code>swap(2,4), swap(1,2), swap(1,5), swap(2,3)</code>。</p>


<pre><code class="language-input2">1
8
8 3 5 7 1 2 4 6
1 1 1 3 1 3 4
</code></pre>


<pre><code class="language-output2">1 3 4 7 5 2 6 8
</code></pre>

<h2>样例三</h2>
<p>见附加文件中 <code>ex_tree3.in</code> 与 <code>ex_tree3.out</code>，该组样例满足子任务 2 的性质。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_tree4.in</code> 与 <code>ex_tree4.out</code>，该组样例满足子任务 3 的性质。</p>
<h2>样例五</h2>
<p>见附加文件中 <code>ex_tree5.in</code> 与 <code>ex_tree5.out</code>，该组样例满足子任务 4 的性质。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据， $1\le n\le 10^5,1\le \mathrm{fa}[i] &lt; i$ ，且保证 $a$ 是一个 $1\sim n$ 的排列。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="3">$2000$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">B</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">$10^5$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">B</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p>特殊性质 A ：令当 $x$ 有多个儿子可选择作为 $u$ 时选择编号最小的策略的 <code>ddm</code> 过程对应 <code>ddm</code> 序 $p_0$，那么有解当且仅当 $p_0$ 合法。</p>
<p>特殊性质 B ：至多只有一个点的儿子个数 $= 2$ ，且不存在儿子个数 $&gt;2$ 的点。换句话说，树 $T$ 的形态形如 “倒 Y” 形。</p>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
