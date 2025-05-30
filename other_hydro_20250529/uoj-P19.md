<p>在有向图 $G$ 中，每条边的长度均为 $1$，现给定起点和终点，请你在图中找一条从起点到终点的路径，该路径满足以下条件：</p>
<ol><li>路径上的所有点的出边所指向的点都直接或间接与终点连通。</li>
<li>在满足条件 1 的情况下使路径最短。</li>
</ol><p>注意：图 $G$ 中可能存在重边和自环，题目保证终点没有出边。</p>
<p>请你输出符合条件的路径的长度。</p>
<h2>输入格式</h2>
<p>第一行有两个用一个空格隔开的整数 $n$ 和 $m$，表示图有 $n$ 个点和 $m$ 条边。</p>
<p>接下来的 $m$ 行每行 $2$ 个整数 $x,y$，之间用一个空格隔开，表示有一条边从点 $x$ 指向点$y$。</p>
<p>最后一行有两个用一个空格隔开的整数 $s, t$，表示起点为 $s$，终点为 $t$。</p>
<h2>输出格式</h2>
<p>输出只有一行，包含一个整数，表示满足题目描述的最短路径的长度。如果这样的路径不存在，输出$-1$。</p>


<pre><code class="language-input1">3 2
1 2
2 1
1 3
</code></pre>


<pre><code class="language-output1">-1
</code></pre>


<p>起点$1$与终点$3$不连通，所以满足题目描述的路径不存在，故输出$-1$。</p>


<pre><code class="language-input2">6 6
1 2
1 3
2 6
2 5
4 5
3 4
1 5
</code></pre>


<pre><code class="language-output2">3
</code></pre>


<p>注意点$2$不能在答案路径中，因为点$2$连了一条边到点$6$，而点$6$不与终点$5$连通。</p>
<h2>限制与约定</h2>
<p>对于30%的数据，$0 &lt; n \le 10$，$0 &lt; m \le 20$;</p>
<p>对于60%的数据，$0 &lt; n \le 100$，$0 &lt; m \le 2000$;</p>
<p>对于100%的数据，$0 &lt; n \le 10000$，$ 0 &lt; m \le 200000$，$0 &lt; x,y,s,t \le n$，$ x,s \ne t$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>内存限制：</strong>$128\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20459/file/attachment.zip">样例数据下载</a></p>
