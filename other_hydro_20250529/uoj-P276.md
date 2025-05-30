<p>牛牛来到了一个盛产汽水的国度旅行。</p>
<p>这个国度的地图上有 $n$ 个城市，这些城市之间用 $n-1$ 条道路连接，任意两个城市之间，都存在一条<strong>路径</strong>连接。这些城市生产的汽水有许多不同的风味，在经过道路 $i$ 时，牛牛会喝掉 $w_i$ 的汽水。牛牛非常喜欢喝汽水，但过量地饮用汽水是有害健康的，因此，他希望在他旅行的这段时间内，<strong>平均每天</strong>喝到的汽水的量尽可能地接近给定的一个正整数 $k$ 。</p>
<p>同时，牛牛希望他的旅行计划尽可能地有趣，牛牛会先选择一个城市作为起点，然后<strong>每天</strong>通过一条道路，前往一个<strong>没有去过</strong>的城市，最终选择在某一个城市结束旅行。</p>
<p>牛牛还要忙着去喝可乐，他希望你帮他设计出一个旅行计划，满足每天$|平均每天喝到的汽水-k|$的值尽量小，请你告诉他这个最小值。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n, k$ 。</p>
<p>接下来 $n - 1$ 行，每行三个正整数 $u_i, v_i, w_i$，表示城市 $u_i$ 和城市 $v_i$ 之间有一条长度为 $w_i$ 的道路连接。</p>
<p>同一行相邻的两个整数均用一个空格隔开。</p>
<h2>输出格式</h2>
<p>一行一个整数，表示 $|平均每天喝到的汽水-k|$ 的最小值<strong>的整数部分</strong>，即你只要将这个最小值<strong>向下取整</strong>然后输出即可。</p>


<pre><code class="language-input1">5 21
1 2 9
1 3 27
1 4 3
1 5 12
</code></pre>


<pre><code class="language-output1">1
</code></pre>


<p>在图中，路径5-&gt;1-&gt;3是一条最合适的路线，总计喝到的汽水的量是 $27 + 12 = 39$, 平均每天喝到的汽水量是 $39 \div 2 = 19.5$, $| 19.5 - 21 | = 1.5$，向下取整后得到 $1$，因此答案是 $1$。</p>
<h2>样例二</h2>
<p>见样例数据下载</p>
<h2>限制与约定</h2>
<p>对于 $20\%$ 的数据，$ n \leq 1000 $。</p>
<p>对于另外 $20\%$ 的数据，保证编号为 $ i (1 \leq i \leq n - 1) $ 的节点和编号为 $i + 1$ 的节点之间连接了一条边。</p>
<p>对于另外 $20\%$ 的数据，保证数据是以1为根的完全二叉树（在完全二叉树中，节点 $ i (2 \leq i \leq n) $ 和节点 $\left \lfloor i \div 2 \right \rfloor$ 之间有一条道路）。</p>
<p>对于另外 $20\%$ 的数据，保证除节点 $1$ 以外，其他节点和节点 $1$ 之间都有一条道路。</p>
<p>对于 $100\%$ 的数据，$1 \le n \le 5 \times 10^{4} , 0 \le w_i \le 10^{13} , 0 \le k \le 10^{13}$。</p>
<p><strong>时间限制</strong>：$5\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20705/file/attachment.zip">样例数据下载</a></p>
