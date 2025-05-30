<p>给定一颗 $n$ 个结点的树，每条边上有一个小写字母。</p>
<p>令 $str(x,y)$ 表示树上 $x$ 到 $y$ 的简单路径上的字母连成的字符串。</p>
<p>定义一个字符串 $T$ 是优秀的，当且仅当 $T$ 能表示成 $SS$ 的形式，其中 $S$ 是一个任意非空字符串。</p>
<p>求树上有多少个<strong>本质不同</strong>的优秀字符串。</p>
<h2>输入格式</h2>
<p>输入第一行一个正整数 $n$，表示树的大小。</p>
<p>接下来 $n-1$ 行，每行形如 $x,y,c$ 表示有一条连接 $(x,y)$ 的边，上面的小写字母是 $c$。</p>
<h2>输出格式</h2>
<p>输出一个非负整数表示答案</p>


<pre><code class="language-input1">5
1 2 a
2 3 a
3 4 b
4 5 b
</code></pre>


<pre><code class="language-output1">2
</code></pre>

<h2>限制与约定</h2>
<p>$2\leq n\leq 5 \times 10^4$</p>
<p><strong>时间限制：</strong>$5\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
