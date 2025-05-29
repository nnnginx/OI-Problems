<p><strong>由于某些原因本题仅支持 C++, C++11 语言的提交。</strong></p>
<p>Grace 是一名生物学家，在新加坡的一个生物信息学公司工作。她的一部分工作是分析不同有机体的 DNA 序列。DNA 序列是包含字符 <code>A</code>、<code>T</code> 和 <code>C</code> 的字符串。注意在本题中，DNA 序列<strong>不包含字符 <code>G</code></strong>。</p>
<p>定义一次修改是把 DNA 序列中的两个元素交换位置的操作。例如，通过交换加粗的字符 <code>A</code> 和 <code>C</code>，一次修改可以把 <code>A<strong>C</strong>T<strong>A</strong></code> 转化为 <code>A<strong>A</strong>T<strong>C</strong></code>。</p>
<p>两个序列的修改距离是把一个序列转化为另一个序列所用的最少修改次数。如果不能通过修改把一个序列转化为另一个序列，那么这两个序列的修改距离为 $-1$。</p>
<p>Grace 正在分析两个 DNA 序列 $a$ 和 $b$，每个都由 $n$ 个元素组成，下标从 $0$ 到 $n - 1$。你的任务是帮助 Grace 回答以下形式的 $q$ 个问题：子串 $a[x \ldots y]$ 和 $b[x \ldots y]$ 的修改距离是多少？这里，DNA 序列 $s$ 的子串 $s[x \ldots y]$ 定义为 $s$ 的下标从 $x$ 到 $y$（包括 $x$ 和 $y$）的连续字符序列。也就是说，$s[x \ldots y]$ 是序列 $s[x] s[x + 1] \ldots s[y]$。]</p>
<h2>实现细节</h2>
<p>你必须引用 <code>dna.h</code> 头文件。</p>
<p>你要实现以下函数：</p>
<pre><code class="sh_cpp">void init(string a, string b)</code></pre>
<ul>
<li>$a, b$：长度为 $n$ 的字符串，表示两个待分析的 DNA 序列。</li>
<li>恰好调用此函数一次，且发生在任何对 <code>get_distance</code> 的调用之前。</li>
</ul>
<pre><code class="sh_cpp">int get_distance(int x, int y)</code></pre>
<ul>
<li>$x, y$：待分析的子串的开始和结束下标。</li>
<li>此函数应返回子串 $a[x \ldots y]$ 和 $b[x \ldots y]$ 的修改距离。</li>
<li>恰好调用此函数 $q$ 次。</li>
</ul>
<h2>输入格式</h2>
<p>评测程序示例按以下格式读取输入：</p>
<ul>
<li>第 $1$ 行：$n \; q$</li>
<li>第 $2$ 行：$a$</li>
<li>第 $3$ 行：$b$</li>
<li>第 $4 + i$（$0 \le i \le q - 1$）行：$x \; y$，是第 $i$ 次调用 <code>get_distance</code> 的参数。</li>
</ul>
<h2>输出格式</h2>
<p>评测程序示例按以下格式打印你的答案：</p>
<ul>
<li>第 $1 + i$（$0 \le i \le q - 1$）行：第 $i$ 次调用 <code>get_distance</code> 的返回值。</li>
</ul>


<pre><code class="language-input1">6 3
ATACAT
ACTATA
1 3
4 5
3 5
</code></pre>


<pre><code class="language-output1">2
1
-1
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">init("ATACAT", "ACTATA")</code></pre>
<p>如果评测程序调用 <code>get_distance(1, 3)</code>，那么该调用应返回 $a[1 \ldots 3]$ 和 $b[1 \ldots 3]$（也就是序列 <code>TAC</code> 和 <code>CTA</code>）之间的修改距离。通过 $2$ 次修改可以把 <code>TAC</code> 转化为 <code>CTA</code>：<code><strong>T</strong>A<strong>C</strong></code> $\to$ <code><strong>C</strong>A<strong>T</strong></code>，然后是 <code>C<strong>AT</strong></code> $\to$ <code>C<strong>TA</strong></code>。无法通过比 $2$ 次更少的修改完成该转化。</p>
<p>因此，该调用应返回 $2$。</p>
<p>如果评测程序调用 <code>get_distance(4, 5)</code>，那么该调用应返回序列 <code>AT</code> 和 <code>TA</code> 之间的修改距离。 通过一次修改可以把 <code>AT</code> 转化为 <code>TA</code>，而且显然至少需要一次。</p>
<p>因此，该调用应返回 $1$。</p>
<p>最后，如果评测程序调用 <code>get_distance(3, 5)</code>，由于<strong>无法</strong>通过修改将序列 <code>CAT</code> 转化为 <code>ATA</code>，因此该调用应返回 $-1$。</p>
<h2>数据范围</h2>
<p>对于所有数据：</p>
<ul>
<li>$1 \le n, q \le 100 \, 000$</li>
<li>$0 \le x \le y \le n - 1$</li>
<li>$a$ 和 $b$ 的每个字符都是 <code>A</code>、<code>T</code> 和 <code>C</code> 之⼀</li>
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
<td style="text-align:center;">$21$</td>
<td style="text-align:center;">$y - x \le 2$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$22$</td>
<td style="text-align:center;">$q \le 500$，$y - x \le 1000$，$a$ 和 $b$ 的每个字符是 <code>A</code> 或 <code>T</code></td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$13$</td>
<td style="text-align:center;">$a$ 和 $b$ 的每个字符是 <code>A</code> 或 <code>T</code></td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$28$</td>
<td style="text-align:center;">$q \le 500$，$y - x \le 1000$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">没有额外的约束条件</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{1s}$</strong></p>
<p><strong>空间限制：$\texttt{2GB}$</strong></p>
