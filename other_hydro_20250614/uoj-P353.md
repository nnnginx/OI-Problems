<p>SingleDog们设法进入了核心，他们发现，三台TPU主机的程序混在了一起，每个主机对应一种颜色，屏幕上出现了斑斓的色条！</p>
<p>具体来说，他们发现了一个长度为$n$的颜色串，每个位置是红/蓝/绿（记为 <samp>R/G/B</samp> ）三个颜色中的一种。为了彻底杜绝AlphaGo的朋友圈狗粮，他们需要把这部分代码完全改写。</p>
<p>根据跳蚤国王发来的消息，每次你可以选择相邻的两个色块，进行一次操作，为了方便理解，记操作前的两个位置的颜色为 $c_a,c_b$ ，操作后的为 $c_a^{'},c_b^{'}$ 。</p>
<ol><li>如果你选择的两个色块是同色（ $c_a=c_b$ ），你可以把它们变成两种<strong>不同的新颜色</strong>（即 $c_a^{'}\neq c_b^{'},c_a\neq c_a^{'},c_b\neq c_b^{'}$ ），例如，当你选择了 <samp>GG</samp> 后，你可以将它们变为 <samp>RB</samp> 或 <samp>BR</samp>。</li>
<li>如果你选择的两个色块是异色（ $c_a\neq c_b$ ），你可以把它们变成两种<strong>相同的新颜色</strong>（即 $c_a^{'}=c_b^{'},c_a\neq c_a^{'},c_b\neq c_b^{'}$ ），例如，当你选择了 <samp>RB</samp> 后，你可以将它们变为 <samp>GG</samp> 。</li>
</ol><p>你的目标是把这串代码从状态 $S$ 变为状态 $T$ ，求最小步数。</p>
<h2>输入格式</h2>
<p>第一行一个正整数 $n$ ，表示这串代码的长度。</p>
<p>第二行一个长度为 $n$ 的字符串 $S$ ，表示这串代码的起始状态。</p>
<p>第三行一个长度为 $n$ 的字符串 $T$ ，表示这串代码的终止状态。</p>
<h2>输出格式</h2>
<p>输出一行一个整数，表示把这串代码从状态 $S$ 变为状态 $T$ 的最小步数。</p>


<pre><code class="language-input1">3
GBR
BBB
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>第一次操作将 <samp>GB</samp> 改为 <samp>RR</samp> ，操作后的代码为 <samp>RRR</samp> 。</p>
<p>第二次操作将 <samp>RR</samp> 改为 <samp>BG</samp> ，操作后的代码为 <samp>BGR</samp> 。</p>
<p>第三次操作将 <samp>GR</samp> 改为 <samp>BB</samp> ，操作后的代码为 <samp>BBB</samp> 。</p>
<p>可以证明没有次数更少的操作序列。</p>


<pre><code class="language-input2">4
GBRB
GRRG
</code></pre>


<pre><code class="language-output2">2
</code></pre>


<p>第一次操作将 <samp>RB</samp> 改为 <samp>GG</samp> ，操作后的代码为 <samp>GBGG</samp> 。</p>
<p>第二次操作将 <samp>BG</samp> 改为 <samp>RR</samp> ，操作后的代码为 <samp>GRRG</samp> 。</p>
<p>可以证明没有次数更少的操作序列。</p>


<pre><code class="language-input3">20
RBBGRBBGRBBBBGRBRGGB
RBGRRBRBGBRRGBBBGBGG
</code></pre>


<pre><code class="language-output3">14
</code></pre>


<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$n$的规模</th>
<th>其他</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$n \leq 10$</td><td rowspan="2">无</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="4">$n = 100$</td><td rowspan="3">存在一种步数不超过 50 且每次操作选取的 $i$ 在 $[1,n-1]$ 中随机的解</td></tr><tr><td>4</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="5">无</td></tr><tr><td>7</td><td rowspan="4">$n\leq 5\times 10^5$</td></tr><tr><td>8</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p>保证 $S$ 和 $T$ 只由大写字母 <samp>'R','G','B'</samp> 组成，保证存在一组操作方案将代码的状态从 $S$ 变为 $T$ 。</p>
<p><strong>时间限制：</strong>$2\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<p>友情提示：题目难度和题目顺序<strong>没有</strong>关系</p>
<h2>下载</h2>
<p><a href="./20779/file/attachment.zip">样例数据下载</a></p>
