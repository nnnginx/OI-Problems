<p>小O和小I一直喜欢打 UOJ 的比赛，然而等了半个丁酉年却也没能等到下一次比赛。眼看着 NOI 即将到来，他们决定一探究竟，找出 UOJ 沉寂的真正原因！</p>
<p>终于有一天，他们得知 UOJ 的管理层全都被两个一心想摧毁 OI 界的大魔王——滴滴诶柳和不响公座给封印起来。</p>
<p>这两个大魔王向来战略上联手对敌，战术上分工合作。每次滴滴诶柳首先给 oier 带来一堆麻烦；接着不响公座用超声波对 oier 进行催眠，降低 oier 们的反抗效率；关键时候滴滴诶柳又进行反向催眠，让 oier 拼命反击筋疲力尽。两个魔王轮流值班，有着充足的休息时间，而他们的对手却受到无间断攻击。最后随着时间的推移，oier 们的体力到了最低点时，不响公座放出大招，将 oier 封印起来。</p>
<p>要想拯救 UOJ，必须打败这两个魔王。小O和小I查阅资料，终于找到了获胜的方法——OI 阵。</p>
<p>首先，他们需要召集 $n$ 名 oier 布阵，联手对敌。为了高效地反击滴滴诶柳，他们决定让 $n$ 名 oier 站成一张图的样子，每个 oier 负责应对自己和相邻 oier 所受到的攻击。当一个 oier 受到攻击时，图中相邻的 oier 及时支援。</p>
<p>同时他们意识到，当一个 oier 身边有同校的 oier 时，不响公座攻击的时候他们会聊起天来从而阵法被破；而反之，如果身边的人都不熟悉，则会产生表现欲，有效抗住不响公座的超声波攻击。<strong>因此他们要求，图中任意两个相邻的 oier 来自不同的学校。</strong></p>
<p>现在已知这张图的构成。该图具有 $n$ 个点 $m$ 条边，节点编号依次为 $1, \dots, n$。同时共有 $k$ 个学校，由于拯救 UOJ 人人有责，故每个学校都有无数的 oier 愿意出力。</p>
<p>小O想要知道有多少种布阵方式，但是鉴于小I最多只能数到 $5$（他学会的最大的数字来自于“一二三四五上山打老虎”），<strong>因此小O决定输出方案数模 6。</strong></p>
<p>两个布阵方式被认为是不同的当且仅当存在一个节点 $i$ 使得这两种布阵方式中守卫该节点的 oier 来自不同的学校。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $T$，表示数据组数。</p>
<p>对于每组数据，第一行三个整数 $n,m,k$，分别表示图的点数、边数、总共的学校数。</p>
<p>接下来 $m$行，每行两个整数 $a,b$，表示 $a,b$ 间有一条边。保证 $1 \le a, b \le n$ 且 $a \neq b$。</p>
<h2>输出格式</h2>
<p>对于每组数据，输出一个数表示该组数据的答案。</p>


<pre><code class="language-inputundefined">2
5 4 5
1 2
1 3
1 4
1 5
8 7 2
1 2
2 3
3 4
4 5
5 6
6 7
7 8
</code></pre>


<pre><code class="language-outputundefined">2
2
</code></pre>

<h2>explanation</h2>
<p>对于第一个数据，五个点形成一个十字路口，根据乘法原理共有 $5 \times 4 \times 4 \times 4 \times 4=1280$ 种布阵法，模 $6$ 余 $2$。</p>
<p>对于第二个数据，构成一个 $8$ 个点的链，当第一个点定好了之后，剩下的全都连锁反应的定好了</p>
<h2>限制与约定</h2>
<p>对全部数据，有 $1\le T \le 5,1\le n \le 10^5,0 \le m \le 2 \times 10^5,1 \le k \le 10000$。图保证无自环。</p>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n$</th><th>$k$</th><th>备注</th>
      </tr></thead><tbody><tr><td>1 ~ 3</td><td>$\le 6$</td><td>$ \le 9$</td><td></td></tr><tr><td>4 ~ 5</td><td>$\leq 10^5$</td><td>$= 1$</td><td></td></tr><tr><td>6</td><td>$\le 10^5$</td><td>$ \le 10^4$</td><td>$m=n-1$，是一棵树</td></tr><tr><td>7~10</td><td>$\le 10^5$</td><td>$\le 10^4$</td><td></td></tr></tbody></table></div>

<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20735/file/attachment.zip">样例数据下载</a></p>
