<p>跳蚤国王成功夺回了管理员权限，并剥夺了 Skip 蚤的权限，让其在 UOJ 上禁赛三年，且所在省的跳蚤 Rating 强制扣$100$。</p>
<p>跳蚤国王在检查题库时，发现 Skip 蚤获得权限期间，一位热爱线段树的 Picks 往 OJ 上传了一道没有 std 的题目。</p>
<p>因为之前的行为引起了民愤，出题人 Picks 拒绝向跳蚤国王透露这题的解法。正巧跳蚤国王准备筹办的 ULR #2 缺一道题，你能帮助跳蚤国王解开这道题以完成 ULR 的筹备吗？</p>
<p>给定一个长度为 $n$ 的操作序列。操作有 4 种：</p>
<ol>
<li><code>| x</code>：将非负整数 $v$ 变为 $v\ \mathrm{bitor}\ x$，其中 $\mathrm{bitor}$ 为按位或操作；</li>
<li><code>&amp; x</code>：将非负整数 $v$ 变为 $v\ \mathrm{bitand}\ x$，其中 $\mathrm{bitand}$ 为按位与操作；</li>
<li><code>^ x</code>：将非负整数 $v$ 变为 $v\ \mathrm{bitxor}\ x$，其中 $\mathrm{bitxor}$ 为按位异或操作；</li>
<li><code>+ x</code>：将非负整数 $v$ 变为 $(v + x) \bmod 2^{32}$。<strong>这一种操作保证 $x=1$。</strong></li>
</ol>
<p>所有操作的 $x$ 均为输入给定的非负整数，每一个操作的 $x$ 并不一定相同。操作从 $0$ 开始编号。</p>
<p>给定 $q$ 次询问，每次给出整数 $v,l,r,t$，求对数 $v$ 依次进行操作序列中区间 $[l,r]$ 中的操作后写成二进制形式，从低到高第 $t+1$ 个二进制位（即表示 $2^t$ 的位）的值，容易发现每组询问的答案只有可能是 $0$ 或 $1$。</p>
<p><strong>本题部分子任务强制在线，详见输入格式和限制与约定部分。</strong></p>
<h2>输入格式</h2>
<p>第一行三个整数 $n,q,op$ 表示操作序列长度、询问个数、询问解密参数。</p>
<p>接下来 $n$ 行依次描述操作序列中的每个元素。每行一个字符 $c$ 表示操作类型，后接一个整数 $x$ 表示操作参数。<strong>对于 <code>+</code> 操作保证 $x=1$。</strong></p>
<p>接下来 $q$ 行每行四个整数 $v',l',r',t'$ 表示一组询问。<strong>注意询问进行了加密</strong>，解密方法如下：</p>
<ul>
<li>设需要解密的询问为第 $t$ 组询问，$ans_i$ 表示第 $i$ 组询问的答案，询问从 $0$ 开始编号； </li>
<li>计算 $\mathrm{key} = op \times (\sum_{i=0}^{t-1} 2^ians_i) \mod 998244353$； </li>
<li>则对应询问的真实参数如下：
\begin{align}
  v &amp;= (v' + \mathrm{key})\bmod 2^{32} \\
 l &amp;= \min\{(l'\ \mathrm{bitxor}\ \mathrm{key})\bmod n,(r'\ \mathrm{bitxor}\ \mathrm{key})\bmod n\} \\
 r &amp;= \max\{(l'\ \mathrm{bitxor}\ \mathrm{key})\bmod n,(r'\ \mathrm{bitxor}\ \mathrm{key})\bmod n\} \\
 t &amp;= (t'\ \mathrm{bitxor}\ \mathrm{key}) \bmod 32
\end{align}</li>
</ul>
<p><strong>注意解密过程中 $v$ 的计算方式与其他三者不同。注意无论询问是否强制在线都需要进行询问解密。</strong></p>
<h2>输出格式</h2>
<p>一行一个长度为 $q$ 的 01 字符串，其中第 $i$ 个字符表示第 $i$ 组询问的答案。</p>


<pre><code class="language-input1">6 6 0
^ 17
+ 1
^ 28
| 6
&amp; 29
+ 1
3 0 2 1
8 1 5 3
7 1 4 0
12 0 4 2
31 0 2 1
50 1 2 0
</code></pre>


<pre><code class="language-output1">100111
</code></pre>


<ul>
<li>第一个询问中有 $3 \xrightarrow[]{\mathrm{bitxor}\ 17} 18 \xrightarrow[]{+1} 19 \xrightarrow[]{\mathrm{bitxor}\ 28} 15 = (1111)_2$，其表示 $2^1$ 的二进制位，即从右往左数第 $2$ 个二进制位的值为 $1$，故第一个询问答案为 $1$；</li>
<li>第二个询问中有 $8 \xrightarrow[]{+1} 9 \xrightarrow[]{\mathrm{bitxor}\ 28} 21 \xrightarrow[]{\mathrm{bitor}\ 6} 23 \xrightarrow[]{\mathrm{bitand}\ 29} 21 \xrightarrow[]{+1} 22 = (10110)_2$，其表示 $2^3$ 的二进制位，即从右往左数第 $4$ 个二进制位的值为 $0$，故第二个询问答案为 $0$。</li>
</ul>


<pre><code class="language-input2">6 6 1
^ 17
+ 1
^ 28
| 6
&amp; 29
+ 1
3 13674554 3172638 395059201
7 6992286 3863695438 3302730626
6 122315987 1653449004 2270895617
11 277356193 306830369 65457603
22 2313889149 858796667 36414120
25 4135467483 3048814434 3407639193
</code></pre>


<pre><code class="language-output2">100111
</code></pre>


<p>该样例解密后即为样例一。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_sequence3.in</code> 与 <code>ex_sequence3.ans</code>，该组样例满足子任务 $1$ 的性质。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_sequence4.in</code> 与 <code>ex_sequence4.ans</code>，该组样例满足子任务 $3$ 的性质。</p>
<h2>样例五</h2>
<p>见附加文件中 <code>ex_sequence5.in</code> 与 <code>ex_sequence5.ans</code>，该组样例满足子任务 $6$ 的性质。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1 \leq n \leq 10^5 , 1 \leq q \leq 6 \times 10^5 , 0 \leq op \leq 1, 0 \leq x,v',l',r',t' &lt; 2^{32}$。保证当操作为 <code>+</code> 操作时 $x=1$。</p>
<table class="table table-bordered table-text-center table-vertical-middle">
<thead><tr><th>子任务编号</th><th>$n \leq $</th><th>$q \leq $</th><th>$op \leq $</th><th>特殊性质</th><th>分值</th></tr></thead>
<tbody>
<tr><td>$1$</td><td>$3000$</td><td>$5000$</td><td>$1$</td><td>无</td><td>$2$</td></tr>
<tr><td>$2$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$0$</td><td>只有 ^,+ 操作</td><td>$8$</td></tr>
<tr><td>$3$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$1$</td><td>只有 ^,+ 操作</td><td>$14$</td></tr>
<tr><td>$4$</td><td>$10^5$</td><td>$4 \times 10^5$</td><td>$1$</td><td>只有 ^,+ 操作</td><td>$16$</td></tr>
<tr><td>$5$</td><td>$10^5$</td><td>$6 \times 10^5$</td><td>$1$</td><td>没有 + 操作</td><td>$6$</td></tr>
<tr><td>$6$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$0$</td><td>无</td><td>$10$</td></tr>
<tr><td>$7$</td><td>$10^5$</td><td>$4 \times 10^5$</td><td>$0$</td><td>无</td><td>$10$</td></tr>
<tr><td>$8$</td><td>$4 \times 10^4$</td><td>$2 \times 10^5$</td><td>$1$</td><td>无</td><td>$14$</td></tr>
<tr><td>$9$</td><td>$10^5$</td><td>$6 \times 10^5$</td><td>$1$</td><td>无</td><td>$20$</td></tr>
</tbody></table>

<p><strong>本题数据中读入的最大文件大小约为 $\texttt{30MB}$，请注意算法常数如读入速度对运行时间带来的影响。</strong></p>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="./21060/file/attachment.zip">样例数据下载</a></p>
