<p>小 D 特别喜欢玩游戏。这一天，他在玩一款填数游戏。</p>
<p>这个填数游戏的棋盘是一个 $n\times m$ 的矩形表格。玩家需要在表格的每个格子中填入一个数字（数字 $0$ 或者数字 $1$），填数时需要满足一些限制。下面我们来具体描述这些限制。</p>
<p>为了方便描述，我们先给出一些定义：</p>
<ul>
<li>我们用每个格子的行列坐标来表示一个格子，即 $(x,y)$，其中，$x$ 为行坐标，$y$ 为列坐标。（注意：行列坐标均从 $0$ 开始编号）；</li>
<li>合法路径 $P$：一条路径是合法的当且仅当：<ol>
<li>这条路径从矩形表格的左上角的格子 $(0,0)$ 出发，到矩形的右下角格子 $(n-1,m-1)$ 结束；</li>
<li>在这条路径中，每次只能从当前的格子移动到右边与它相邻的格子，或者从当前格子移动到下面与它相邻的格子。</li>
</ol>
</li>
</ul>
<p>例如：在下面这个矩形中，只有两条路径是合法的，它们分别是 $P_1:(0,0)\to (0,1)\to (1,1), \ P_2:(0,0)\to (1,0)\to (1,1)$。</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/440/tianshu1.webp" alt="示意图" style="width:400px;"></p>
<p>对于一条合法的路径 $P$，我们可以用一个字符串 $w(P)$ 来表示，该字符串的长度为 $n+m-2$，其中只包含字符 <code>R</code> 或者字符 <code>D</code>，第 $i$ 个字符记录了路径 $P$ 中第 $i$ 步的移动方法，<code>R</code> 表示移动到当前格子右边与它相邻的格子，<code>D</code> 表示移动到当前格子下面与它相邻的格子。例如，上图中对于路径 $P_1$，有 $w(P_1)=``\text{RD}"$；而对于另一条路径 $P_2$，有 $w(P_2)=``\text{DR}"$。</p>
<p>同时，将每条合法路径 $P$ 经过的每个格子上填入的数字依次连接后，会得到一个长度为 $n+m-1$ 的 $01$ 字符串，记为 $s(P)$。例如，如果我们在格子 $(0,0)$ 和 $(1,0)$ 上填入数字 $0$，在格子 $(0,1)$ 和 $(1,1)$ 上填入数字 $1$（见上图红色数字）。那么对于路径 $P_1$，我们可以得到 $s(P_1)=``011"$，对于路径 $P_2$，有 $s(P_2)=``001"$。</p>
<p>游戏要求小 D 找到一种填数字 $0,1$ 的方法，使得对于两条路径 $P_1,P_2$，如果 $w(P_1)\gt w(P_2)$，那么必须 $s(P_1)\le s(P_2)$。我们说字符串 $a$ 比字符串 $b$ 小，当且仅当字符串 $a$ 的字典序小于字符串 $b$ 的字典序，字典序的定义详见<a href="/problem/439">第一题</a>。但是仅仅是找一种方法无法满足小 D 的好奇心，小 D 更想知道这个游戏有多少种玩法，也就是说，有多少种填数字的方法满足游戏的要求？</p>
<p>小 D 能力有限，希望你帮助他解决这个问题，即有多少种填 $0,1$ 的方法能满足题目要求。由于答案可能很大，你需要输出答案对 $10^9+7$ 取模的结果。</p>
<h2>输入格式</h2>
<p>输入文件，包含两个正整数 $n,m$，由一个空格分隔，表示矩形的大小。其中 $n$ 表示矩形表格的行数，$m$ 表示矩形表格的列数。</p>
<h2>输出格式</h2>
<p>输出共一行，包含一个正整数，表示有多少种填 $0,1$ 的方法能满足游戏的要求。</p>
<p>注意：输出答案对 $10^9+7$ 取模的结果。</p>


<pre><code class="language-input1">2 2
</code></pre>
<pre><code class="language-output1">12
</code></pre><h4>样例说明 1</h4>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/440/tianshu2.png" alt="示意图" style="width:800px;"></p>
<p>对于 $2\times 2$ 棋盘，有上图所示的 $12$ 种填数方法满足要求。</p>


<pre><code class="language-input2">3 3
</code></pre>
<pre><code class="language-output2">112
</code></pre>

<pre><code class="language-input3">5 5
</code></pre>
<pre><code class="language-output3">7136
</code></pre><h2>限制与约定</h2>
<p>对于所有子任务均满足 $1\ \leq\ n,m$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-verticle-middle">
<thead>
  <tr><th>测试点编号</th><th>$n\le$</th><th>$m\le$</th></tr></thead>
  <tbody><tr><td>$1\sim 4$</td><td>$3$</td><td>$3$</td></tr><tr><td>$5\sim 10$</td><td>$2$</td><td>$10^6$</td></tr><tr><td>$11\sim 13$</td><td>$3$</td><td>$10^6$</td></tr><tr><td>$14\sim 16$</td><td>$8$</td><td>$8$</td></tr><tr><td>$17\sim 20$</td><td>$8$</td><td>$10^6$</td></tr></tbody>
</table>
</div>

<p><strong>时间限制：$\texttt{1s}$。</strong></p>
<p><strong>空间限制：$\texttt{512MB}$。</strong></p>
<h2>下载</h2>
<p><a href="./20845/file/attachment.zip">样例数据下载</a></p>
