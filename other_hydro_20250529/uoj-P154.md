<p>picks 博士通过实验成功地得到了排列 $A$，并根据这个回到了正确的过去。他在金星凌日之前顺利地与丘比签订了契约，成为了一名马猴烧酒。</p>
<p>picks 博士可以使用魔法召唤很多很多的猴子与他一起战斗，但是当猴子的数目 $n$ 太大的时候，训练猴子就变成了一个繁重的任务。</p>
<p>历经千辛万苦，猴子们终于学会了按照顺序排成一排。为了进一步训练，picks 博士打算设定一系列的指令，每一条指令 $i$ 的效果都可以用一个 $1$ 到 $n$ 的排列 $P_i$ 表示，picks 博士希望喊出这条指令之后，猴子们能够自行交换顺序，使得之前排在第 $j$ 个的猴子在交换结束后排在第 $P_{i,j}$的位置。</p>
<p>因为实战时争分夺秒，他认为一个完善的指令系统必须满足如下的条件：</p>
<ol><li>对于任意的两条指令 $i$ 和 $j$ ($i$ 和 $j$ 可以相同)，在指令系统中一定存在一条指令 $k$，使得依次喊出第 $i$ 条指令和第 $j$ 条指令的效果和直接喊出第 $k$ 条指令的效果是一样的。picks 博士认为这样可以提高战场上发号施令的效率。</li>
<li>任意两条不同指令 $i$ 和 $j$ 的效果是不同的。picks 博士认为这样可以避免指令系统过于臃肿。</li>
</ol><p>现在 picks 博士已经完成了对指令系统大致的构思。具体来说，他已经得到了一个整数 $m$ 以及一个 $m \times m$ 的表格 $B$。整数 $m$ 表示指令系统中指令的数量，$B_{i,j}$ 表示依次喊出第 $i$ 条指令和第 $j$ 条指令的效果和直接喊出第 $B_{i,j}$ 条指令的效果是一样的。</p>
<p>现在 picks 博士想要根据 $m$ 和 $B$ 来得到一个完善的指令系统。然而他发现这样的指令系统有很多，这引起了他的兴趣，他想要你帮他统计满足条件的完善的指令系统究竟有多少个。</p>
<p>两个指令系统是不同的当且仅当至少存在一个 $i$ 使得两个指令系统中的第 $i$ 条指令不同。</p>
<p>不保证一定存在满足条件的完善的指令系统，毕竟聪慧过人的马猴烧酒 picks 博士也有搞错的时候嘛。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $T$，表示数据组数。</p>
<p>对于每组数据，第一行是两个正整数 $n$ 和 $m$，表示猴子的数量以及指令系统的指令数量。</p>
<p>接下来 $m$ 行每行 $m$ 个正整数 $B_{i,j}$，表示依次喊出第 $i$ 条指令和第 $j$ 条指令的效果和直接喊出第 $B_{i,j}$ 条指令的效果是一样的。保证有$1 \leq B_{i,j} \leq m$。</p>
<h2>输出格式</h2>
<p>对于每组数据输出一个整数表示答案。</p>
<p>答案可能很大，你只需要输出答案对 $998244353（7\times 17 \times 2^{23}+1$，一个质数$）$ 取模后的结果。</p>


<pre><code class="language-input1">1
3 2
1 2
2 1
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>可能的三种指令系统为：</p>
<ol><li>第一个指令为排列 $1\ 2\ 3$，第二个指令为排列 $1\ 3\ 2$。</li>
<li>第一个指令为排列 $1\ 2\ 3$，第二个指令为排列 $2\ 1\ 3$。</li>
<li>第一个指令为排列 $1\ 2\ 3$，第二个指令为排列 $3\ 2\ 1$。</li>
</ol><h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$m$ 的规模</th><th>$n$ 的规模</th><th>其他</th></tr></thead><tbody><tr><td>1</td><td rowspan="2">$m \leq 4$</td><td rowspan="2">$n \leq 5$</td><td rowspan="2"></td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="2">$m \leq 30$</td><td rowspan="8">$n \leq 1000$</td><td rowspan="2">$B_{i,j} \equiv i+j-1 \pmod{m}$</td></tr><tr><td>4</td></tr><tr><td>5</td><td rowspan="3">$m \leq 16$</td><td rowspan="6"></td></tr><tr><td>6</td></tr><tr><td>7</td></tr><tr><td>8</td><td rowspan="3">$m \leq 30$</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>对于所有数据，保证有 $T \leq 10$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20594/file/attachment.zip">样例数据下载</a></p>
