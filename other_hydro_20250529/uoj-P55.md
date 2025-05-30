<div class="hide">
$\newcommand\xor{\mathbin{\mathrm{xor}}}$
</div>

<p>强强和萌萌是一对好朋友。有一天他们在外面闲逛，突然看到前方有一棵紫荆树。这已经是紫荆花飞舞的季节了，无数的花瓣以肉眼可见的速度从紫荆树上长了出来。</p>
<p>仔细看看的话，这个大树实际上是一个带权树。每个时刻它会长出一个新的叶子节点，每个节点上有一个可爱的小精灵，新长出的节点上也会同时出现一个新的小精灵。小精灵是很萌但是也很脆弱的生物，每个小精灵 $i$ 都有一个感受能力值 $r_i$，小精灵 $i, j$ 成为朋友当且仅当在树上 $i$ 和 $j$ 的距离 $\text{dist}(i, j) \leq r_i + r_j$，其中 $\text{dist}(i, j)$ 表示在这个树上从 $i$ 到 $j$ 的唯一路径上所有边的边权和。</p>
<p>强强和萌萌很好奇每次新长出一个叶子节点之后，这个树上总共有几对朋友。</p>
<p>我们假定这个树一开始为空，节点按照加入的顺序从 $1$ 开始编号。由于强强非常好奇，你必须在他每次出现新结点后马上给出总共的朋友对数，不能拖延哦。</p>
<h2>输入格式</h2>
<p>第一行包含一个整数，表示测试点编号。</p>
<p>第二行包含一个正整数 $n$，表示总共要加入的节点数。</p>
<p>我们令加入节点前的总共朋友对数是 $\text{last_ans}$，在一开始时它的值为 $0$。</p>
<p>接下来 $n$ 行中第 $i$ 行有三个非负整数 $a_i, c_i, r_i$，表示结点 $i$ 的父节点的编号为 $a_i \xor (\text{last_ans} \bmod 10^9)$（其中 $\xor$ 表示异或，$\bmod$表示取余，数据保证这样操作后得到的结果介于 $1$ 到 $i - 1$ 之间），与父结点之间的边权为 $c_i$，节点 $i$ 上小精灵的感受能力值为 $r_i$。</p>
<p>注意 $a_1 = c_1 = 0$，表示 $1$ 号节点是根结点，对于 $i &gt; 1$，父节点的编号至少为 $1$。</p>
<h2>输出格式</h2>
<p>包含 $n$ 行，每行输出 $1$ 个整数，表示加入第 $i$ 个点之后，树上有几对朋友。</p>


<pre><code class="language-input1">0
5
0 0 6
1 2 4
0 9 4
0 5 5
0 2 4
</code></pre>


<pre><code class="language-output1">0
1
2
4
7
</code></pre>

<h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<p>对于所有数据，满足 $1 \leq c_i \leq 10000$，$a_i \leq 2 \times 10^9$，$r_i \leq 10^9$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>约定</th></tr></thead><tbody><tr><td>1, 2</td><td>$n \leq 100$</td></tr><tr><td>3, 4</td><td>$n \leq 1000$</td></tr><tr><td>5, 6, 7, 8</td><td>$n \leq 100000$，节点 $1$ 最多有两个子节点，其它节点最多有一个子节点</td></tr><tr><td>9, 10</td><td>$n \leq 100000$，$r_i \leq 10$</td></tr><tr><td>11, 12</td><td>$n \leq 100000$，这棵树是随机生成的</td></tr><tr><td>13, 14, 15</td><td>$n \leq 70000$</td></tr><tr><td>16, 17, 18, 19, 20</td><td>$n \leq 100000$</td></tr></tbody></table></div>

<p>此题 hack 时忽略输入数据中给定的测试点编号对测试点的限制。</p>
<p>祝大家一遍 AC，求不虐萌萌哒测评机！</p>
<p><strong>时间限制</strong>：$12\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20495/file/attachment.zip">样例数据下载</a></p>
