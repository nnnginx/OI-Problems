<p>Cyberland 有 $n$ 座城市，编号从 $1$ 到 $n$，有 $m$ 条双向道路连接这些城市。第 $j$ 条路连接城市 $a_j$ 和 $b_j$。每天，都有成千上万的游客来到 Cyberland 游玩。</p>
<p>在每一个城市，都有纪念品售卖，第 $i$ 个城市售价为 $w_i$。这个售价有时会变动。</p>
<p>每一个游客的游览路径都有固定起始城市和终止城市，且不会经过重复的城市。</p>
<p>他们会在路径上的城市中，售价最低的那个城市购买纪念品。</p>
<p>你能求出每一个游客在所有合法的路径中能购买的最低售价是多少吗？</p>
<p>你要处理 $q$ 个操作：</p>
<ul><li><code>C a w</code>： 表示 $a$ 城市的纪念品售价变成 $w$。</li>
<li><code>A a b</code>： 表示有一个游客要从 $a$ 城市到 $b$ 城市，你要回答在所有他的旅行路径中最低售价的最低可能值。</li>
</ul><h2>输入格式</h2>
<p>第一行包含用一个空格隔开的三个数，$n$、$m$、$q$。</p>
<p>接下来 $n$ 行，每行包含一个数 $w_i$。</p>
<p>接下来 $m$ 行，每行包含用一个空格隔开的两个数 $a_j$, $b_j$。（$1 \le a_j, b_j \le n, a_j \ne b_j$）</p>
<p><strong>数据保证没有两条道路连接同样一对城市，也没有一条道路两端是相同的城市。并且任意两个城市都可以相互到达。</strong></p>
<p>接下来 $q$ 行，每行是<code>C a w</code> 或 <code>A a b</code> ，描述了一个操作。</p>
<h2>输出格式</h2>
<p>对于每一个<code>A</code>类操作，输出一行表示对应的答案。</p>


<pre><code class="language-input1">3 3 3
1
2
3
1 2
2 3
1 3
A 2 3
C 1 5
A 2 3
</code></pre>


<pre><code class="language-output1">1
2
</code></pre>



<pre><code class="language-input2">7 9 4
1
2
3
4
5
6
7
1 2
2 5
1 5
2 3
3 4
2 4
5 6
6 7
5 7
A 2 3
A 6 4
A 6 7
A 3 3
</code></pre>


<pre><code class="language-output2">2
1
5
3
</code></pre>



<p>一种可能的最优路径是：</p>
<ul><li>2, 3</li>
<li>6, 5, 1, 2, 4</li>
<li>6, 5, 7</li>
<li>3</li>
</ul><h2>限制与约定</h2>
<p>$1 \le n, m,q \le 10^5$，$ 1 \le w_i \le 10^9$</p>
<p><strong>时间限制：</strong>$2\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20470/file/attachment.zip">样例数据下载</a></p>
