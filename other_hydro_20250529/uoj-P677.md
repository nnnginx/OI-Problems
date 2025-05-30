<p>Yelekastee 是 U 国著名的考古学家。在最近的一次考古行动中，他发掘出了一个远古时期的密码箱。经过周密而严谨的考证，Yelekastee 得知密码箱的密码和某一个数列 $\{ a_n \}$ 相关。数列 $\{ a_n \}$ 可以用如下方式构造出来：</p>
<ol>
<li>初始时数列长度为 $2$ 且有 $a_0 = 0, a_1 = 1$；</li>
<li>对数列依次进行若干次操作，其中每次操作是以下两种类型之一：<ul>
<li><code>W</code> 类型：给数列的<strong>最后一项</strong>加 $1$。</li>
<li><code>E</code> 类型：若数列的<strong>最后一项</strong>为 $1$，则给倒数第二项加 $1$；否则先给数列的<strong>最后一项</strong>减 $1$，接着在数列尾再加两项，两项的值都是 $1$。</li>
</ul>
</li>
</ol>
<p>受到技术限制，密码箱并没有办法完整检查整个数列，因此密码箱的密码设定为数列 $\{ a_n \}$ 经过函数 $f$ 作用后的值，其中 $f$ 的定义如下：</p>
<p>$$ f(a_0, \ldots , a_{k - 1}, a_k) = \begin{cases} a_0, &amp; k = 0 \\ f \left( a_0, a_1, \ldots , a_{k - 2}, a_{k - 1} + \frac{1}{a_k} \right) , &amp; k \ge 1 \end{cases} $$</p>
<p>Yelekastee 并不擅长运算，因此他找到了你，希望你能根据他提供的操作序列计算出密码箱的密码。不幸的是，他的记性并不是很好，因此他会随时对提供的操作序列做出一些修改，这些修改包括以下三种：</p>
<ul>
<li><code>APPEND c</code>，在现有操作序列后追加一次 <code>c</code> 类型操作，其中 <code>c</code> 为字符 <code>W</code> 或 <code>E</code>。</li>
<li><code>FLIP l r</code>，反转现有操作序列中第 $l$ 个至第 $r$ 个（下标从 $1$ 开始，修改包含端点 $l$ 和 $r$，下同）操作，即所有 <code>W</code> 变为 <code>E</code>，所有 <code>E</code> 变为 <code>W</code>。</li>
<li><code>REVERSE l r</code>，翻转现有操作序列中第 $l$ 个至第 $r$ 个操作，也就是将这个区间中的操作逆序。</li>
</ul>
<h2>输入格式</h2>
<p>输入第一行包含两个正整数 $n, q$，分别表示初始的操作序列长度和修改的次数。</p>
<p>第二行包含一个长为 $n$ 且仅包含大写字母 <code>W</code> 和 <code>E</code> 的字符串，表示初始操作序列。</p>
<p>接下来 $q$ 行，每行表示一次修改。每种修改的格式如题目描述所述。</p>
<h2>输出格式</h2>
<p>输出共 $q + 1$ 行，每行两个整数，其中第一行表示初始操作序列对应的密码，接下来 $q$ 行则分别输出每次修改之后的操作序列对应的密码。</p>
<p>容易发现密码一定是正有理数。若真实的密码为 $\frac{a}{b}$，其中 $a, b &gt; 0$ 且 $\gcd(a, b) = 1$，则你需要在对应的行内顺次输出 $a$ 和 $b$ 模 $998244353$ 后的余数。</p>


<pre><code class="language-input1">2 3
WE
APPEND E
FLIP 1 2
REVERSE 2 3
</code></pre>


<pre><code class="language-output1">2 3
3 4
5 3
5 2
</code></pre>


<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">$ $</th>
<th style="text-align:center;">操作序列</th>
<th style="text-align:center;">数列 $\{ a_n \}$</th>
<th style="text-align:center;">密码</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">初始</td>
<td style="text-align:center;"><code>WE</code></td>
<td style="text-align:center;">$(0, 1, 1, 1)$</td>
<td style="text-align:center;">$\frac{2}{3}$</td>
</tr>
<tr>
<td style="text-align:center;">第一次修改后</td>
<td style="text-align:center;"><code>WEE</code></td>
<td style="text-align:center;">$(0, 1, 2, 1)$</td>
<td style="text-align:center;">$\frac{3}{4}$</td>
</tr>
<tr>
<td style="text-align:center;">第二次修改后</td>
<td style="text-align:center;"><code>EWE</code></td>
<td style="text-align:center;">$(1, 1, 1, 1)$</td>
<td style="text-align:center;">$\frac{5}{3}$</td>
</tr>
<tr>
<td style="text-align:center;">第三次修改后</td>
<td style="text-align:center;"><code>EEW</code></td>
<td style="text-align:center;">$(2, 2)$</td>
<td style="text-align:center;">$\frac{5}{2}$</td>
</tr>
</tbody>
</table>
</div>
<h2>样例二</h2>
<p>见附加文件中的 <code>ex_code2.in</code> 与 <code>ex_code2.ans</code>。</p>
<p>该样例与测试数据 $1 \sim 4$ 满足同样的约束条件。</p>
<h2>样例三</h2>
<p>见附加文件中的 <code>ex_code3.in</code> 与 <code>ex_code3.ans</code>。</p>
<p>该样例与测试数据 $ 5 \sim 7$ 满足同样的约束条件。</p>
<h2>样例四</h2>
<p>见附加文件中的 <code>ex_code4.in</code> 与 <code>ex_code4.ans</code>。</p>
<p>该样例与测试数据 $8 \sim 10$ 满足同样的约束条件。</p>
<h2>样例五</h2>
<p>见附加文件中的 <code>ex_code5.in</code> 与 <code>ex_code5.ans</code>。</p>
<p>该样例与测试数据 $15 \sim 20$ 满足同样的约束条件。</p>
<h2>测试点约束</h2>
<p>对于所有测试点：$1 \le n \le {10}^5$，$1 \le q \le {10}^5$。</p>
<p>对于 <code>APPEND</code> 修改，保证给出的 <code>c</code> 为大写英文字母 <code>W</code> 或 <code>E</code>。</p>
<p>对于 <code>FLIP</code> 和 <code>REVERSE</code> 修改，保证 $1 \le l \le r \le L$，其中 $L$ 是当前操作序列的长度。</p>
<p>请注意由于有 <code>APPEND</code> 操作，操作序列的长度最大可能有 $2 \times {10}^5$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n, q \le$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 7$</td>
<td style="text-align:center;">${10}^5$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$8 \sim 10$</td>
<td style="text-align:center;">${10}^5$</td>
<td style="text-align:center;">B，C</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 14$</td>
<td style="text-align:center;">${10}^5$</td>
<td style="text-align:center;">C</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 20$</td>
<td style="text-align:center;">${10}^5$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p>特殊限制 A：保证在任意时刻操作序列中不会出现连续相同的两个字符。</p>
<p>特殊限制 B：保证没有 <code>FLIP</code> 修改。</p>
<p>特殊限制 C：保证没有 <code>REVERSE</code> 修改。</p>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{1GB}$</strong></p>
