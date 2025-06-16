<p>蒜斜曾经也是一个 OI 选手。</p>
<p>那是大概五年前的故事了，在那个时候，虽然 CN OI 还不一定是 Best OI，但是 CN DS 早就已经是 Best DS 了。作为一名做着 BZOJ 长大的选手，蒜斜曾经也能两分钟写一棵线段树，五分钟写一棵平衡树，闭着眼睛写动态树。</p>
<p>转眼间五年过去，CN OI 已经变成了当之无愧的 Best OI。受到今年 IOI 中国队辉煌成绩的鼓舞，蒜斜打算时隔多年再来做几道数据结构题，感受一下当年的青葱岁月。</p>
<p>然而，世界最大的垃圾数据结构批发基地 BZOJ 早已宣布停止运营，落后于时代的蒜斜一下子不知道到哪去找数据结构题来做。</p>
<p>于是，他悄摸摸地回到了当年算法竞赛圈最大的交流平台 Universal OJ 用户群打算碰碰运气。巧的是，他一进群，就看到有一位热心群友在出数据结构题。</p>
<p><img src="https://img.uoj.ac/problem/637/image.png" alt="造数据结构图" class="img-responsive center-block"></p>
<p>这是一道看上去就很有趣的题目。给定一个长度为 $n$ 的序列 $a$，序列的标号从 $1$ 开始，每一个位置是一个 $[1,n]$ 内的整数。有 $m$ 个操作，每次操作给出一个区间 $[l,r]$：这次操作会先将下标在 $[l,r]$ 中的所有元素加上 $1$，然后询问全局颜色数，并在最后撤销这次修改（也就是说操作之间互不影响）。其中，一个序列的全局颜色数定义为这个序列中出现的不同数值的个数。</p>
<p>虽然蒜斜曾经也很擅长数据结构，但是岁月带走了 BZOJ，捎走了蒜斜在 BZOJ 上的所有代码，也顺带着送走了蒜斜的算法竞赛水平。因此，他希望你能帮他解决一下这道题目。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $n,m$。</p>
<p>第二行 $n$ 个用空格隔开的数表示序列 $a (1 \leq a_i \leq n)$。</p>
<p>之后 $m$ 行，每行两个用空格隔开的数 $l,r (1 \leq l \leq r \leq n)$ 表示一次询问。</p>
<h2>输出格式</h2>
<p>对每个操作，输出一行一个数表示答案。</p>


<pre><code class="language-inputundefined">10 10
3 10 5 9 1 10 6 4 6 8
4 5
1 6
3 4
2 9
2 7
5 6
8 9
8 9
5 8
1 9
</code></pre>


<pre><code class="language-outputundefined">7
6
6
8
8
9
8
8
9
8
</code></pre>

<h2>限制与约定</h2>
<p><strong>Small Task</strong>: $1\le n\le 5000, 1 \le m \le 10^6$。</p>
<p><strong>Large Task</strong>: $1\le n,m \le 10^6$。</p>
<p><strong>时间限制：</strong>$2\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21038/file/attachment.zip">样例数据下载</a></p>
