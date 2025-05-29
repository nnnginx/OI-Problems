<p>Bob 喜欢字符串。</p>
<p>Bob 觉得，重复两遍的字符串是优美的，例如，<code>aa</code>、<code>sese</code>、<code>abcabc</code>、<code>baabaa</code>、<code>abababab</code> 是优美的串，而 <code>ab</code>、<code>aadead</code>、<code>sesese</code>、<code>abba</code> 不是。更具体地说，如果一个字符串 $S$ 能够被写成两个相同的字符串前后拼接的形式，即存在字符串 $P$ 使得 $S = PP$，那么 $S$ 就是优美的。</p>
<p>Bob 有一个长度为 $n$ 的字符串 $T = T_1 T_2 \cdots T_n$。现在他想知道，给定 $T$ 的一个子串 $Q = T[l \dots r]$，这个子串 $Q$ 内一共包含多少种本质不同的优美的串作为子串。如果两个串相同，但是出现的位置不同，那么这两个串不是本质不同。</p>
<p>Bob 一共有 $q$ 组不同的询问，你需要快速计算出答案。</p>
<h2>输入格式</h2>
<p>第一行输入两个整数 $n, q$。第二行输入一个只包含小写字母 $a$ 和 $b$ 的字符串 $T$。</p>
<p>接下来 $q$ 行，每行输入两个整数 $l, r$，表示一组询问。</p>
<h2>输出格式</h2>
<p>输出 $q$ 行，每行一个整数表示答案。</p>


<pre><code class="language-input1">11 5
aabaabaaaab
1 11
1 6
7 10
5 5
3 8
</code></pre>


<pre><code class="language-output1">5
2
2
0
2
</code></pre>


<p>$|T|$ 有 <code>aa</code>、<code>aaaa</code>、<code>abaaba</code>、<code>aabaab</code>、<code>baabaa</code> 这些本质不同的优美的串。</p>
<h2>样例二</h2>
<p>见附加文件中 <code>ex_string2.in</code> 与 <code>ex_string2.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于前 $10\%$ 的数据，$n\le 100$。</p>
<p>对于前 $20\%$ 的数据，$n\le 500$。</p>
<p>对于前 $40\%$ 的数据，$n\le 5000$。</p>
<p>对于另外 $20\%$ 的数据，保证 $T$ 中所有的优美的串的个数不超过 $10^6$，这里位置不同的串被视为不同的。</p>
<p>对于另外 $20\%$ 的数据，$q = 1$。</p>
<p>对于 $100\%$ 的数据，$1\le n, q\le 2\times 10^5, 1\le l\le r\le n$，$T$ 只包含小写字母 <code>a</code> 和 <code>b</code>。</p>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20988/file/attachment.zip">样例数据下载</a></p>
