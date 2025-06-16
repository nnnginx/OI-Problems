<p>可怜发现了一种快速构造超长字符串的方法。</p>
<p>最开始，可怜手上有一个空串 $s_0$，接着，可怜对这个串进行了 $n$ 次操作。在第 $i$ 次操作的时候，可怜选择了一个字符 $c$，并利用 $s_{i-1}$ 和 $c$ 构造了字符串 $s_i = cs_{i-1}[1]cs_{i-1}[2] \dots s_{i-1}[m]c$，其中 $m$ 为串 $s_{i-1}$ 的长度。</p>
<p>举例来说，如果 $n=3$ 且可怜选择的字符分别是 $a,b,c$，则 $s_n=cbcacbc$。</p>
<p>现在，可怜想要知道，字符串 $s_n$ 本质不同的非空子序列有多少个。（注意不能为空，但可能是 $s_n$ 本身）。</p>
<p>串 $s$ 是串 $t$ 的子序列当且仅当串 $s$ 可以通过删去 $t$ 中的某些字符得到。</p>
<h2>输入格式</h2>
<p>第一行输入一个整数 $n(1 \leq n \leq 2000)$，表示可怜进行的操作次数。</p>
<p>第二行输入一个长度为 $n$ 的小写字符串 $s$，其中 $s_i$ 表示可怜在第 $i$ 轮选择的字符。</p>
<h2>输出格式</h2>
<p>输出一行一个答案，表示 $s_n$ 中本质不同的子序列个数，答案可能很大，对 $998244353$ 取模后输出。</p>


<pre><code class="language-input1">2
ab
</code></pre>


<pre><code class="language-output1">6
</code></pre>



<pre><code class="language-input2">10
aaaaaaaaaa
</code></pre>


<pre><code class="language-output2">1023
</code></pre>


<h2>限制与约定</h2>
<p><strong>Small Task</strong>: $n\leq 20$。</p>
<p><strong>Large Task</strong>: $n \leq 2000$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20921/file/attachment.zip">样例数据下载</a></p>
