<p>零点的钟声敲响，猴年终于到来啦~</p>
<p>在这新年的第一天，猴族首领猴腮雷打算让你——他的大内总管来帮他整理一下他库存的腮雷。</p>
<p>你发现猴族首领猴腮雷的仓库里有 $n$ 颗腮雷。每颗腮雷有一个威力（均为正整数），我们用 $a_1, a_2, \cdots, a_n$ 表示。</p>
<p>整理腮雷的方法比较特殊：每次，你可以选择 $m$ 颗腮雷（$m \geq 2$），将这些腮雷合并成一颗威力更大的腮雷。具体来说，我们有参数 $b_1, b_2, \cdots, b_m$（均为正整数）。比如你这次选择的 $m$ 颗腮雷的威力为 $x_1, x_2, \cdots, x_m$，那么合并以后，原来的 $m$ 颗腮雷会消失，而会产生一颗威力为 $\max\{x_1+b_1, x_2+b_2, \cdots, x_m+b_m\}$ 的腮雷。</p>
<p>你需要进行若干次合并，直到不能再合并为止。<strong>保证有 $(n-1) \bmod (m-1)=0$，所以最后会剩下恰好一颗腮雷。</strong></p>
<p>其实你的真实身份是跳蚤国派来的间谍，借此机会你打算削弱猴族的军事实力，所以你的目标是让最后剩下的这颗腮雷的威力最小。</p>
<p><strong>为了方便，你不必输出方案，只需要输出这个最小值即可。</strong></p>
<h2>输入格式</h2>
<p>第一行两个正整数：$n, m$。</p>
<p>第二行 $n$ 个正整数，依次表示 $a_1, a_2, \cdots, a_n$。</p>
<p>第三行 $m$ 个正整数，依次表示 $b_1, b_2, \cdots, b_m$。</p>
<h2>输出格式</h2>
<p>只输出一个数，表示最后剩下的腮雷的威力的最小值。</p>


<pre><code class="language-input1">3 2
3 2 3
2 1
</code></pre>


<pre><code class="language-output1">5
</code></pre>


<p>初始的腮雷威力为 $\{3,2,3\}$，每次可以合并$2$颗腮雷，设其威力为 $x_1,x_2$，则产生的腮雷的威力为 $\max(x_1+2,x_2+1)$。</p>
<p>一种最优的方案是：首先合并威力为 $2$ 和 $3$ 的腮雷，得到威力为 $4$ 的腮雷。（注意，如果反过来合并，威力将会是 $5$）然后再合并威力为 $3$ 和 $4$ 的腮雷，得到威力为 $5$ 的腮雷。此时仅剩的一颗腮雷威力为 $5$。并且，不存在更优的方案了。</p>


<pre><code class="language-input2">3 2
10 15 20
1 10
</code></pre>


<pre><code class="language-output2">25
</code></pre>


<p>一种最优方案是：先合并 $20$ 和 $10$ 得到 $21$，然后再合并 $21$ 和 $15$ 得到 $25$。</p>
<h2>样例三</h2>
<p>见样例数据下载。这组数据符合子任务 3 的限制与约定。</p>
<h2>限制与约定</h2>
<p>由于一些原因，本题使用捆绑测试。每个子任务有若干个测试点，分为 $9$ 个子任务，你只有通过一个子任务的所有测试点才能得到这个子任务的分数。</p>
<p>对于所有的数据：$1 \leq n \leq 50000, 2 \leq m \leq 50000, (n - 1) \bmod (m - 1) = 0, 1 \leq a_i \leq 10^8, 1 \leq b_i \leq 10^7$。</p>
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务</th><th>分值</th><th colspan="2">限制与约定</th></tr></thead><tbody><tr><td>1</td><td>13</td><td colspan="2">$n, a_i, b_i \leq 7$</td></tr><tr><td>2</td><td>11</td><td colspan="2">$n = m$</td></tr><tr><td>3</td><td>24</td><td colspan="2">$a_1 = a_2 = \cdots = a_n$</td></tr><tr><td>4</td><td>6</td><td>$m = 2, b = \{1, 1\}$</td><td rowspan="4">$n=49981$<br>$1 \leq a_i \leq 20$且是等概率随机生成的</td></tr><tr><td>5</td><td>5</td><td>$m = 3, b = \{1, 2, 2\}$</td></tr><tr><td>6</td><td>9</td><td>$m = 5, b = \{1, 1, 2, 2, 2\}$</td></tr><tr><td>7</td><td>4</td><td>$m = 5, b = \{2, 2, 2, 3, 3\}$</td></tr><tr><td>8</td><td>12</td><td colspan="2">$n, a_i, b_i \leq 50$</td></tr><tr><td>9</td><td>16</td><td colspan="2">没有特殊的限制与约定</td></tr></tbody></table><p><strong>时间限制：$2\texttt{s}$</strong></p>
<p><strong>空间限制：$256\texttt{MB}$</strong></p>
<h2>下载</h2>
<p><a href="./20617/file/attachment.zip">样例数据下载</a></p>
