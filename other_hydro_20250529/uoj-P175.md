<p>零点的钟声敲响，猴年终于到来啦~</p>
<p>在这新年的第一天，猴族首领猴腮雷打算来整治一下网络风气。这时，他听说在一个叫做 Universal OJ 用户群 的 QQ 群中有人在散播（开）谣言（车），于是他就派了一群网警把这个用户群里的人都抓了回来，试图找到谣言的源头。</p>
<p>这个用户群中有 $n$ 个人，这些人中存在 $m$ 对双向的直接认识关系，<strong>这个社交网络中任意两个人都是直接或者间接认识的</strong>。经过研究，谣言的散播以如下的方式进行：</p>
<ol><li>首先在某个时刻 $T$，谣言的源头想出了一个谣言，于是他在时刻 $T + 1$ 把这个谣言讲给了所有和他直接认识的人听。</li>
<li>如果一个人在第 $i$ 个时刻第一次听到了这个谣言，他会在第 $i + 1$ 时刻时把这个谣言讲给所有和他直接认识的人听。</li>
</ol><p>现在网警们问出来每一个人第一次听到这个谣言的时间，但是遗憾的是<strong>他们并不知道 $T$ 的具体数值</strong>。而且，谣言的发起者不会坐以待毙，他可以随便回答一个时间（当然也可以回答真实时间），而<strong>其他不是谣言的源头的人一定不会撒谎</strong>。（注意：<strong>网警知道谣言的发起者可以说谎</strong>）</p>
<p>猴族首领猴腮雷根据网警们递交上来的口供，非常轻易的就推理出了谣言的源头是谁并把他绳之以法。但是他发现，有些情况下，根据口供还不能唯一确定嫌疑人（即嫌疑人可能有多个），于是他想要知道哪些人是“安全的谣言发起人”。</p>
<p>一个人是安全的谣言发起人，当且仅当他可以通过捏造口供使得猴腮雷无法唯一确定嫌疑人（具体可以看样例解释）。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $T$，表示数据组数。</p>
<p>对于每组数据，第一行包含两个正整数 $n$ 和 $m$。</p>
<p>接下来 $m$ 行每行两个整数 $u$ 和 $v$ 表示第 $u$ 个人和第 $v$ 个人认识。保证 $1 \leq u, v \leq n$ 且 $u \neq v$ 且任意两个人的认识关系至多被描述一遍。</p>
<h2>输出格式</h2>
<p>对于每组数据，第一行输出一个正整数，表示安全谣言发起人数目 $K$。</p>
<p>第二行输出 $K$ 个从小到大的正整数，表示这 $K$ 个发起人的编号。</p>


<pre><code class="language-input1">3
2 1
1 2
5 5
1 2
2 3
3 4
4 5
5 1
3 3
1 2
2 3
3 1
</code></pre>


<pre><code class="language-output1">2
1 2
0

3
1 2 3
</code></pre>


<p>对于第一组数据：</p>
<ol><li>第一个人在时刻 $7000$ 时散布谣言，并撒谎他是在时刻 $7001$ 时听到的，这时他就安全了。</li>
<li>第二个人在时刻 $7000$ 时散布谣言，并撒谎他是在时刻 $7001$ 时听到的，这时他就安全了。</li>
</ol><p>对于第三组数据：</p>
<ol><li>第一个人在时刻 $998244352$ 时散布谣言，并撒谎他是在时刻 $998244353$ 时听到的，这时他就安全了。</li>
<li>第二个人在时刻 $998244352$ 时散布谣言，并撒谎他是在时刻 $998244353$ 时听到的，这时他就安全了。</li>
<li>第三个人在时刻 $998244352$ 时散布谣言，并撒谎他是在时刻 $998244353$ 时听到的，这时他就安全了。</li>
</ol><h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n$ 的规模</th><th>$m$ 的规模</th></tr></thead><tbody><tr><td>1</td><td rowspan="3">$n \leq 200$</td><td rowspan="10">$m \leq 2 \times 10^5$</td></tr><tr><td>2</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="3">$n \leq 2000$</td></tr><tr><td>5</td></tr><tr><td>6</td></tr><tr><td>7</td><td rowspan="4">$n \leq 100000$</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>对于所有数据，保证 $1 \leq T \leq 5$，$n \geq 2$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20615/file/attachment.zip">样例数据下载</a></p>
