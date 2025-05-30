<p>给定一个大小为 $n$ 的树,它共有 $n$ 个结点与 $n − 1$ 条边,结点从 $1 \sim n$ 编号。初始时每个结点上都有一个 $1 \sim n$ 的数字,且每个 $1 \sim n$ 的数字都只在<strong>恰好</strong>一个结点上出现。</p>
<p>接下来你需要进行<strong>恰好</strong> $n − 1$ 次删边操作,每次操作你需要选一条<strong>未被删去</strong>的边，此时这条边所连接的两个结点上的数字将会<strong>交换</strong>,然后这条边将被删去。</p>
<p>$n − 1$ 次操作过后,所有的边都将被删去。此时,按数字从小到大的顺序,将数字 $1 \sim n$ 结点编号依次排列,就得到一个结点编号的排列 $P_i$。现在请你求出,在最优操作方案下能得到的<strong>字典序最小</strong>的 $P_i$。</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/490/csptree1.webp" style="width:200px;" alt="示意图"></p>
<p>如上图,蓝圈中的数字 $1 \sim 5$ 一开始分别在结点②、①、③、⑤、④。按照 (1)(4)(3)(2)的顺序删去所有边,树变为下图。按数字顺序得到的结点编号排列为①、③、④、②、⑤。排列是所有可能的结果中字典序最小的。</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/490/csptree2.webp" style="width:230px;" alt="示意图"></p>
<h2>输入格式</h2>
<p><strong>本题输入包含多组测试数据。</strong></p>
<p>第一行一个正整数 $T$ ,表示数据组数。</p>
<p>对于每组测试数据:</p>
<p>第一行一个整数 $n$,表示树的大小。</p>
<p>第二行 $n$ 个整数,第 $i(1 \leq i \leq n)$ 个整数表示数字 $i$ 初始时所在的结点编号。</p>
<p>接下来 $n − 1$ 行每行两个整数 $x, y$,表示一条连接 $x$ 号结点与 $y$ 号结点的边。</p>
<h2>输出格式</h2>
<p>对于每组测试数据,输出一行共 $n$ 个用空格隔开的整数,表示最优操作方案下所能得到的字典序最小的 $P_i$ 。</p>


<pre><code class="language-inputundefined"><code class="sh_plain">4
5
2 1 3 5 4
1 3
1 4
2 4
4 5
5
3 4 2 1 5
1 2
2 3
3 4
4 5
5
1 2 5 3 4
1 2
1 3
1 4
1 5
10
1 2 3 4 5 7 8 9 10 6
1 2
1 3
1 4
1 5
5 6
6 7
7 8
8 9
9 10</code>
</code></pre>

<pre><code class="language-outputundefined"><code class="sh_plain">1 3 4 2 5
1 3 5 2 4
2 3 1 4 5
2 3 4 5 6 1 7 8 9 10</code>
</code></pre>
<h2>样例2</h2>
<p>见下发文件。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n \leq $</th><th>特殊性质</th></tr></thead><tbody><tr><td>$1 \sim 2$</td><td>$10$</td><td></td></tr><tr><td>$3 \sim 4$</td><td>$160$</td><td rowspan="2">树的形态是一条链</td></tr><tr><td>$5 \sim 7$</td><td>$2000$</td></tr><tr><td>$8 \sim 9$</td><td>$160$</td><td rowspan="2">存在度数为$n-1$的点</td></tr><tr><td>$10 \sim 12$</td><td>$2000$</td></tr><tr><td>$13 \sim 16$</td><td>$160$</td><td rowspan="2"></td></tr><tr><td>$17 \sim 20$</td><td>$2000$</td></tr></tbody></table></div>

<p>对于所有测试点: $1 \leq T \leq 10$,保证给出的是一个树。</p>
<p><strong>时间限制:</strong> $2\texttt{s}$</p>
<p><strong>空间限制:</strong> $256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20895/file/attachment.zip">样例数据下载</a></p>
