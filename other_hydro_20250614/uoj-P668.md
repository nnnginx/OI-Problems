<p>UOI 的一道构造题是一个外星草履虫出的，难度很低。</p>
<p>给定一棵 $n$ 个点的有标号无根树 $T$ 和一个正整数 $k$，我们可以给 $T$ 上的节点染上编号为 $0$ 到 $k$ 的 $k+1$ 种颜色。</p>
<p>宇宙浩瀚而无穷，大部分空间都是空的，因此颜色基本全是 $0$ 的染色方案更可能阐明了宇宙的本质。我们称一个染色方案为 $k$ 元染色方案，当且仅当存在一个由 $1$ 到 $n$ 中的 $k$ 个互不相同的整数组成的序列 $(a_1, a_2, \dots, a_k)$，使得 $T$ 中节点 $a_i$ 的颜色恰为 $i$，而其他未出现在序列中的节点颜色均为 $0$。请你构造一个 $k$ 元染色方案。</p>
<p>大D米轻松解决了这道题。然而，竞赛委员会认为，不同选手思路不一样，不可能构造出<strong>本质相同</strong>的方案。因此，如果两个选手方案本质相同，他们会被判为作弊。</p>
<p>这里定义两个 $k$ 元染色方案是<strong>本质相同</strong>的，若存在一个 $1$ 到 $n$ 的排列 $(p_1, \dots, p_n)$，使第一个方案中 $T$ 的每个节点 $i$ 的颜色均与第二个方案中节点 $p_i$ 的颜色相同，且在第一个方案中 $x,y$ 之间有边当且仅当在第二个方案中 $p_x,p_y$ 之间有边。</p>
<p>大D米想知道自己因此痛失 AK 的概率，于是你需要对 $k=1\sim n$ 分别求出<strong>本质不同</strong>的 $k$ 元染色方案个数，答案对 $998244353$ 取模。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $n$。</p>
<p>接下来 $n-1$ 行，每行两个正整数 $u_i,v_i$，表示 $T$ 的一条边 $(u_i,v_i)$。</p>
<h2>输出格式</h2>
<p>输出一行 $n$ 个整数，第 $i$ 个整数表示本质不同的 $i$ 元染色方案数目对 $998244353$ 取模的值。</p>


<pre><code class="language-input1">4
1 2
1 3
1 4
</code></pre>


<pre><code class="language-output1">2 3 4 4
</code></pre>


<p>注意到在本质相同的意义下，$2,3,4$ 号节点是没有区别的，但跟 $1$ 号节点均有区别。因此本质不同的方案只取决于 $1$ 号点染的颜色，当 $k &lt; n$ 时有 $k+1$ 种可能的颜色，当 $k = n$ 时则有 $k$ 种可能的颜色。</p>


<pre><code class="language-input2">6
3 1
4 6
5 3
2 1
4 5
</code></pre>


<pre><code class="language-output2">3 15 60 180 360 360
</code></pre>

<h2>样例三</h2>
<p>见附加文件中 <code>ex_color3.in</code> 与 <code>ex_color3.out</code>，该组样例满足子任务 2 的性质。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_color4.in</code> 与 <code>ex_color4.out</code>，该组样例满足子任务 3 的性质。</p>
<h2>样例五</h2>
<p>见附加文件中 <code>ex_color5.in</code> 与 <code>ex_color5.out</code>，该组样例满足子任务 5 的性质。</p>
<h2>样例六</h2>
<p>见附加文件中 <code>ex_color6.in</code> 与 <code>ex_color6.out</code>，该组样例满足子任务 7 的性质。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1 \leq n\leq 10^5$，$1\leq u_i,v_i\leq n$，保证给定的边构成一棵树。</p>
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
<td style="text-align:center;">$7$</td>
<td style="text-align:center;" rowspan="3">无</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$300$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;" rowspan="2">$10^5$</td>
<td style="text-align:center;">$u_i=i,v_i=i+1$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$5\times 10^4$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$20$</td>
</tr>
</tbody>
</table>
</div>
<p>特殊性质 A：给定的有标号无根树在所有 $n$ 个节点的有标号无根树中等概率随机生成。</p>
<p><strong>时间限制：$\texttt{1s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
