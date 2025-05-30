<p>一条东西走向的穆西河将巴邻旁市一分为二，分割成了区域 $A$ 和区域 $B$。</p>
<p>每一块区域沿着河岸都建了恰好 $1000000001$ 栋的建筑，每条岸边的建筑都从 $0$ 编号到 $1000000000$。相邻的每对建筑相隔 $1$ 个单位距离，河的宽度也是 $1$ 个单位长度。区域 $A$ 中的 $i$ 号建筑物恰好与区域 $B$ 中的 $i$ 号建筑物隔河相对。</p>
<p>城市中有 $N$ 个居民。第 $i$ 个居民的房子在区域 $P_i$ 的 $S_i$ 号建筑上，同时他的办公室坐落在 $Q_i$ 区域的 $T_i$ 号建筑上。一个居民的房子和办公室可能分布在河的两岸，这样他就必须要搭乘船只才能从家中去往办公室，这种情况让很多人都觉得不方便。为了使居民们可以开车去工作，政府决定建造不超过 $K$ 座横跨河流的大桥。</p>
<p>由于技术上的原因，每一座桥必须刚好连接河的两岸，桥梁必须严格垂直于河流，并且桥与桥之间不能相交。</p>
<p>当政府建造最多 $K$ 座桥之后，设 $D_i$ 表示第 $i$ 个居民此时开车从家里到办公室的最短距离。请帮助政府建造桥梁，使得 $D_1 + D_2 + \dots + D_N$ 最小。</p>
<h2>输入格式</h2>
<p>输入的第一行包含两个正整数 $K$ 和 $N$，分别表示桥的上限数量和居民的数量。</p>
<p>接下来 $N$ 行，每一行包含四个参数：$P_i, S_i, Q_i$ 和 $T_i$，表示第 $i$ 个居民的房子在区域 $P_i$ 的 $S_i$ 号建筑上，且他的办公室位于 $Q_i$ 区域的 $T_i$ 号建筑上。</p>
<h2>输出格式</h2>
<p>输出仅为一行，包含一个整数，表示 $D_1 + D_2 + \dots + D_N$ 的最小值。</p>


<pre><code class="language-input1">1 5
B 0 A 4
B 1 B 3
A 5 B 7
B 2 A 6
B 1 A 7
</code></pre>


<pre><code class="language-output1">24
</code></pre>



<pre><code class="language-input2">2 5
B 0 A 4
B 1 B 3
A 5 B 7
B 2 A 6
B 1 A 7
</code></pre>


<pre><code class="language-output2">22
</code></pre>

<h2>子任务</h2>
<p>所有数据都保证：$P_i$ 和 $Q_i$ 为字符 “<samp>A</samp>” 和 “<samp>B</samp>” 中的一个， $0 \leq S_i, T_i \leq 1000000000$，同一栋建筑内可能有超过 $1$ 间房子或办公室（或二者的组合，即房子或办公室的数量同时大于等于 $1$）。</p>
<ul><li>子任务 1 （8 分）<ul><li>$K = 1$</li>
<li>$1 \leq N \leq 1000$</li>
</ul></li>
<li>子任务 2 （14 分）<ul><li>$K = 1$</li>
<li>$1 \leq N \leq 100000$</li>
</ul></li>
<li>子任务 3 （9 分）<ul><li>$K = 2$</li>
<li>$1 \leq N \leq 100$</li>
</ul></li>
<li>子任务 4 （32 分）<ul><li>$K = 2$</li>
<li>$1 \leq N \leq 1000$</li>
</ul></li>
<li>子任务 5 （37 分）<ul><li>$K = 2$</li>
<li>$1 \leq N \leq 100000$</li>
</ul></li>
</ul><p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20552/file/attachment.zip">样例数据下载</a></p>
