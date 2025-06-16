<p>小 C 学习完了字符串匹配的相关内容，现在他正在做一道习题。</p>
<p>对于一个字符串 $S$，题目要求他找到 $S$ 的所有具有下列形式的拆分方案数: $S = ABC, S = ABABC, S = ABAB \cdots ABC$，其中 $A,B,C$ 均是非空字符串，且 $A$ 中出现奇数次的字符数量不超过 $C$ 中出现奇数次的字符数量。</p>
<p>更具体地，我们可以定义 $AB$ 表示两个字符串 $A, B$ 相连接，例如 $A = \texttt{aab}, B = \texttt{ab}$， 则 $AB = \texttt{aabab}$。</p>
<p>并递归地定义 $A^1 = A, A^n = A^{n−1}A$（$n \ge 2$ 且为正整数）。例如 $A = \texttt{abb}$，则 $A^3 = \texttt{abbabbabb}$。</p>
<p>则小 C 的习题是求 $S = (AB)^iC$ 的方案数，其中 $F(A) \le F(C)$，$F(S)$ 表示字符串 $S$ 中出现奇数次的字符的数量。两种方案不同当且仅当拆分出的 $A$、$B$、$C$ 中有至少一个字符串不同。</p>
<p>小 C 并不会做这道题，只好向你求助，请你帮帮他。</p>
<h2>输入格式</h2>
<p>本题有多组数据，输入的第一行一个正整数 $T$ 表示数据组数。</p>
<p>每组数据仅一行一个字符串 $S$，意义见题目描述。$S$ 仅由英文小写字母构成。</p>
<h2>输出格式</h2>
<p>对于每组数据输出一行一个整数表示答案。</p>


<pre><code class="language-input1">3
nnrnnr
zzzaab
mmlmmlo
</code></pre>


<pre><code class="language-output1">8
9
16
</code></pre>

<h2>样例解释一</h2>
<p>对于第一组数据，所有的方案为: </p>
<ol>
<li>$A=\texttt{n}$，$B=\texttt{nr}$，$C=\texttt{nnr}$。</li>
<li>$A=\texttt{n}$，$B=\texttt{nrn}$，$C=\texttt{nr}$。</li>
<li>$A=\texttt n$，$B=\texttt{nrnn}$，$C=\texttt r$。</li>
<li>$A=\texttt{nn}$，$B=\texttt r$，$C=\texttt{nnr}$。</li>
<li>$A=\texttt{nn}$，$B=\texttt{rn}$，$C=\texttt{nr}$。</li>
<li>$A=\texttt{nn}$，$B=\texttt{rnn}$，$C=\texttt r$。</li>
<li>$A=\texttt{nnr}$，$B=\texttt n$，$C=\texttt{nr}$。</li>
<li>$A=\texttt{nnr}$，$B=\texttt{nn}$，$C=\texttt r$。</li>
</ol>


<pre><code class="language-input2">15
kkkkkkkkkkkkkkkkkkkk
lllllllllllllrrlllrr
cccccccccccccxcxxxcc
ccccccccccccccaababa
ggggggggggggggbaabab
</code></pre>


<pre><code class="language-output2">156
138
138
147
194
</code></pre>

<h2>样例三</h2>
<p>见附加文件中的 <code>ex_string3.in/ans</code>。</p>
<h2>样例四</h2>
<p>见附加文件中的 <code>ex_string4.in/ans</code>。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$\lvert S \rvert \le$</th>
<th style="text-align:center;">特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 4$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 8$</td>
<td style="text-align:center;">$100$</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 12$</td>
<td style="text-align:center;">$1000$</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 14$</td>
<td style="text-align:center;">$2^{15}$</td>
<td style="text-align:center;">$S$ 中只包含一种字符</td>
</tr>
<tr>
<td style="text-align:center;">$15 \sim 17$</td>
<td style="text-align:center;">$2^{16}$</td>
<td style="text-align:center;">$S$ 中只包含两种字符</td>
</tr>
<tr>
<td style="text-align:center;">$18 \sim 21$</td>
<td style="text-align:center;">$2^{17}$</td>
</tr>
<tr>
<td style="text-align:center;">$22 \sim 25$</td>
<td style="text-align:center;">$2^{20}$</td>
</tr>
</tbody>
</table>
</div>
<p>对于所有测试点，保证 $1\le T\le5$，$1\le |S|\le 2^{20}$。</p>
<p><strong>时间限制</strong>：$1 \texttt{s}$</p>
<p><strong>空间限制</strong>：$512 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20985/file/attachment.zip">附加文件下载</a></p>
