<p>零点的钟声马上就要敲响，2016 年即将要拉开序幕，元旦老人轻手轻脚地来到了 <span class="uoj-username" data-rating="1500">jiry_2</span> 的床头，准备把他的礼物装进袜子里。</p>
<p>然而，<span class="uoj-username" data-rating="1500">jiry_2</span> 的礼物居然是一个汉诺塔！汉诺塔怎么才能装进袜子里呢？这让元旦老人犯了难。</p>
<p>经过研究，元旦老人发现：只有当汉诺塔上圆盘的状态是 $T$ 时，这个汉诺塔才能被装进袜子里！然而留给元旦老人的时间已经所剩无几了，情急之下，他决定向你寻求帮助：</p>
<p>给出一个有 $n$ 个圆盘的汉诺塔，一开始汉诺塔的状态为 $S$，接着你可以对这个汉诺塔进行至多 $m$ 次移动，要求在移动结束之后汉诺塔的状态是 $T$，请问不同的操作序列有多少种？</p>
<p>两个操作序列时不同的当且仅当操作序列长度不同或者在某一步操作之后汉诺塔的状态不同。</p>
<p>一个汉诺塔由三根柱子和若干个大小互不相同的圆盘组成，每一次操作你可以取出某一根柱子上最顶端的圆盘然后放到另外一根的柱子的顶端，同时必须保证每一时刻每一个圆盘不能放在比它小的圆盘的上方。</p>
<p>如果你对题面还有疑惑，请结合样例解释食用。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n,m$。</p>
<p>第二行是 $n$ 个 $1$ 到 $3$ 之间的正整数 $A_i$，描述了状态 $S$：$A_i$ 表示第 $i$ 小的圆盘处在第 $A_i$ 根柱子上。</p>
<p>第三行是 $n$ 个 $1$ 到 $3$ 之间的正整数 $B_i$，描述了状态 $T$：$B_i$ 表示第 $i$ 小的圆盘处在第 $B_i$ 根柱子上。</p>
<p>同一根柱子上的圆盘默认为以自上而下大小递增的顺序摆放。</p>
<h2>输出格式</h2>
<p>第一行输出一个整数，表示合法的操作序列数目。</p>
<p>答案可能很大，你只需要输出答案对 $998244353（7\times 17 \times 2^{23}+1$，一个质数$）$ 取模后的结果。</p>


<pre><code class="language-input1">1 2
1
3
</code></pre>


<pre><code class="language-output1">2
</code></pre>


<p>你可以一步把这个圆盘移到第三根柱子上，也可以先移动到中间，再移动到第三根柱子上。</p>


<pre><code class="language-input2">2 4
1 1
1 2
</code></pre>


<pre><code class="language-output2">4
</code></pre>


<p>四种操作序列如下：</p>
<ol><li>先把第一个圆盘放到第三根柱子上，再把第二个圆盘放到第二根柱子上，最后再把第一个圆盘放回去。</li>
<li>先把第一个圆盘放到第三根柱子上，再把第二个圆盘放到第二根柱子上，接着把第一个圆盘放到第二根柱子上，最后再把它放回去。</li>
<li>先把第一个圆盘放到第二根柱子上，再把它放到第三根柱子上，接着把第二个圆盘放到第二根柱子上，最后再把第一个圆盘放回去。</li>
<li>先把第一个圆盘放到第二根柱子上，再把第二个圆盘放到第三根柱子上，接着把第一个圆盘放回去，最后把第二个圆盘放到第二根柱子上。</li>
</ol>

<pre><code class="language-input3">1 2
1
1
</code></pre>


<pre><code class="language-output3">3
</code></pre>


<p>要么保持不动，要么先移动到第二根（第三根）柱子上，再移动回来。</p>


<pre><code class="language-input4">3 10
1 1 1
2 1 3
</code></pre>


<pre><code class="language-output4">149
</code></pre>

<h2>样例五</h2>
<p>见样例数据下载。</p>
<h2>样例六</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n$ 的规模</th><th>$m$ 的规模</th></tr></thead><tbody><tr><td>1</td><td>$n \leq 3$</td><td rowspan="3">$m \leq 10$</td></tr><tr><td>2</td><td rowspan="2">$n \leq 50$</td></tr><tr><td>3</td></tr><tr><td>4</td><td rowspan="2">$n \leq 10$</td><td rowspan="5">$m \leq 50$</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="3">$n \leq 50$</td></tr><tr><td>7</td></tr><tr><td>8</td></tr><tr><td>9</td><td rowspan="2">$n \leq 100$</td><td rowspan="2">$m \leq 100$</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20607/file/attachment.zip">样例数据下载</a></p>
<h2>新年快乐！</h2>
<p>2016，好好做人。</p>
