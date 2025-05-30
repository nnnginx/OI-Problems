<p>一番战斗之后，程序猿被计算鸡们赶走了。随着垫子计算鸡一声令下：“追！”，于是计算鸡村全村上下开始乘胜追击。计算鸡们希望在新的一年到来之际给程序猿以重创，出掉这一年的恶气。</p>
<p>可是程序猿一追就走，一走就跑，一跑就无影无踪。计算鸡们开始跋山涉水寻找程序猿的踪迹。快乐游戏鸡跟随大部队走着走着，突然说道：“我好像打过类似的游戏”。</p>
<p>快乐游戏鸡玩过的游戏是这样的：给定一棵 $n$ 个结点的树，其中 $1$ 号结点是根。每次玩家可以在树上行走，走过一条边需要 $1$ 秒的时间，但只能往当前所在的点的某个儿子走，不能往父亲走。每次游戏需要从 $s$ 号结点走到 $t$ 号结点去。</p>
<p>玩家有一个总死亡次数，初始为 $0$。每个结点上有一个程序猿和一个参数 $w_i$，如果走到结点 $i$ 的时候，当前总的死亡次数小于 $w_i$，那么玩家就会立刻死亡并回到起点 $s$，且该死亡过程不需要时间；如果总死亡次数大于等于 $w_i$，那么玩家就能熟练地对付程序猿从而安然无恙。<strong>注意每次游戏时不需要考虑 $s$ 和 $t$ 上的程序猿。</strong></p>
<p>该游戏会进行若干轮，每轮会清空总死亡次数并给出一组新的 $s, t$。现在请你对于每一轮游戏输出走到 $t$ 所需要的最短时间（单位为秒）。</p>
<p>保证每个询问的 $s$ 可以到达 $t$。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $n$，表示树的结点数。</p>
<p>第二行 $n$ 个正整数，其中第 $i$ 个表示 $w_i$。</p>
<p>第三行 $n-1$ 个整数，第 $i$ 个表示 $i+1$ 号点的父亲结点 $f_i$，保证 $f_i &lt; i$ 。</p>
<p>第四行一个正整数 $q$ 表示游戏轮数。</p>
<p>接下来 $q$ 行，每行两个整数 $s,t$，表示一轮游戏。</p>
<h2>输出格式</h2>
<p>输出 $q$ 行，每行一个整数表示每轮游戏的答案。</p>


<pre><code class="language-input1">5
1 1 2 4 4
1 1 2 4
1
1 5
</code></pre>


<pre><code class="language-output1">9
</code></pre>


<p>由于题面提到每次询问 $s,t$ 的时候不考虑 $s$ 和 $t$ 上的程序猿，所以首先我们无视点 $1$ 和点 $5$ 的程序猿。</p>
<p>一种可能的方案：</p>
<ol><li>死亡次数为 $0$ 时，从点 $1$ 走到点 $2$ 碰到程序猿，死亡，回到点 $1$，耗时 $1$ 秒；</li>
<li>死亡次数为 $1$ 时，从点 $1$ 走到点 $3$ 碰到程序猿，死亡，回到点 $1$，耗时 $1$ 秒；</li>
<li>死亡次数为 $2$ 时，从点 $1$ 走到点 $4$ 碰到程序猿，死亡，回到点 $1$，耗时 $2$ 秒；</li>
<li>死亡次数为 $3$ 时，从点 $1$ 走到点 $4$ 碰到程序猿，死亡，回到点 $1$，耗时 $2$ 秒；</li>
<li>死亡次数为 $4$ 时，从点 $1$ 走到点 $5$，耗时 $3$ 秒。</li>
</ol><p>总耗时 $9$ 秒。</p>


<pre><code class="language-input2">8
10 4 2 3 1 6 2 7
1 2 3 4 1 6 7
5
1 5
1 8
2 4
2 5
3 3
</code></pre>


<pre><code class="language-output2">8
9
4
7
0
</code></pre>

<h2>样例三</h2>
<p>见样例数据下载。该样例满足子任务 $2$ 条件。</p>
<h2>样例四</h2>
<p>见样例数据下载。该样例满足子任务 $4$ 条件。</p>
<h2>限制与约定</h2>
<p>由于一些原因，本题使用捆绑测试。每个子任务有若干个测试点，分为 5 个子任务，你只有通过一个子任务的所有测试点才能得到这个子任务的分数。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务</th>
<th>分值</th>
<th>$n$</th>
<th>其它限制</th>
</tr></thead><tbody><tr><td>1</td><td>10</td><td>$\leq 1000$</td><td>$q \leq 10$ ， $w_i \leq 100$</td></tr><tr><td>2</td><td>10</td><td>$\leq 5000$</td><td>$q \leq 5000$</td></tr><tr><td>3</td><td>20</td><td rowspan="3">$\leq 3 \times 10^5$</td><td>对于所有询问，保证 $s=1$</td></tr><tr><td>4</td><td>30</td><td>对于所有 $i \geq 2$ ，保证 $f_i = i-1$</td></tr><tr><td>5</td><td>30</td><td>无</td></tr></tbody></table></div>

<p>对于所有数据，保证 $1 \leq n,q \leq 3 \times 10^5$ 且 $1 \leq w_i \leq 10^9$ 且 $f_i &lt; i$ 且 $1 \leq s,t \leq n$。</p>
<p><strong>时间限制：</strong>$2\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20713/file/attachment.zip">样例数据下载</a></p>
