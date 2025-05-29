<p>得到了蛐蛐国王的援助后，跳蚤国王率领大量蛐蛐回到了跳蚤国，很快聚拢起了旧部。几次胜利后，跳蚤国王几乎将跳晚国军队完全驱逐出了跳蚤国境内，剩余一部分精锐跳晚在跳跳将军率领下在坚固的堡垒跳跳堡负隅顽抗。为了攻克跳跳堡，跳蚤国王派你——伏特潜入跳跳堡打探情报。</p>
<p>然而你在潜入的时候被抓住了。你被带到了跳跳将军的面前，跳跳将军找到了数学高手小 L，他表示你要是能和他玩游戏并获胜，就能放你走，一共三次机会。</p>
<p>第一次是在竞赛图中轮流找 Hamilton 链，小 L 先手获胜。第二次是给一个最小点度为 $k$ 的无向图和一棵 $k$ 个点的树，你要从图中找出 $k$ 个点，使它们生成子图包含这棵树，且删掉这 $k$ 个点后图仍连通。由于过于紧张，你忘记要保证连通。</p>
<p>现在是最后一次机会了，但是题目也更为复杂：</p>
<p>定义一个简单无向图 $G$ 是“优美”的，当且仅当对 $G$ 中任意四个不同点 $A,B,C,D$，若 $AB,BC,CD$ 间均有边，则 $AC,BD,AD$ 间不可能同时没有边（即要么 $AC$ 有边，要么 $BD$ 有边，要么 $AD$ 有边）。</p>
<p><img src="https://img.uoj.ac/problem/632/632.png" alt="例子" class="img-responsive center-block" style="width:400px;"></p>
<p>例如上面图片左边的图是“优美”的；而右边的图若取 $A=1,B=2,C=4,D=5$ ，则 $AB,BC,CD$ 间均有边，且 $AC,BD,AD$ 间均没有边，因此不是一个“优美”的图。</p>
<p>给定一个 $n$ 个点的“优美”的简单无向图 $G$ ，你要对所有 $i=1, \dots, n$，求出 $G$ 中有多少个点集子集的生成子图同构于 $K_i$，其中 $K_i$ 代表 $i$ 个点的完全图。也就是说，对于任意一个 $i$，你都要求出 $G$ 中有多少个大小为 $i$ 的点的集合，使得集合中任意两点均在 $G$ 中有直接的边相连。你只需要告诉跳跳将军答案对 $998244353$ 取模的值。</p>
<p>容易发现，这个问题不会比计算 $G$ 中最大团大小容易。</p>
<p>你发现这个问题心算是肯定做不出来的，但跳跳将军给你提供了一台计算机，你需要用计算机解决它。</p>
<p><strong>提示：你只需要解决第三个问题，前两个问题与本题没有任何关系</strong>。</p>
<h2>输入格式</h2>
<p><strong>为了减小输入量，本题对输入进行了压缩</strong>。</p>
<p>第一行一个正整数 $n$，表示一个“优美”的图 $G$ 的点数。</p>
<p>接下来 $n-1$ 行，第 $i$ 行为一个长度为 $\lceil \frac{n-i}{4} \rceil$ 的字符串，仅包含 <samp>'0'</samp> ~ <samp>'9'</samp> 和 <samp>'A'</samp> ~ <samp>'F'</samp>。这里，字符 <samp>'0'</samp>~<samp>'9'</samp> 依次对应整数 $0\sim 9$，<samp>'A'</samp>~<samp>'F'</samp> 依次对应整数 $10\sim 15$。 </p>
<p>对 $\forall 1\leq j\leq n-i$，$G$ 中边 $(i,i+j)$ 存在当且仅当该字符串第 $\lceil \frac{j}{4} \rceil$ 个字符所对应整数的二进制表示下从低往高第 $(j-1) \bmod 4$ 位为 $1$，注意若 $(n-i) \bmod 4\neq 0$，则最后一个字符二进制表示下没有定义的位一定为 $0$。</p>
<h2>输出格式</h2>
<p>输出一行 $n$ 个用空格分开的整数，第 $i$ 个整数为 $G$ 点集子集的生成子图中同构于 $K_i$ 的个数对 $998244353$ 取模的值。</p>


<pre><code class="language-input1">4
5
1
1
</code></pre>


<pre><code class="language-output1">4 4 0 0
</code></pre>


<p>对输入解压后，得到的 $G$ 的邻接矩阵为</p>
<pre>0101
1010
0101
1010
</pre>

<p>这是一个 $4$ 个点的环，有边 $(1,2),(2,3),(3,4),(4,1)$，描述的图为题目描述图片中的左图。</p>
<p>容易看出它的最大团大小为 $2$，且各有 $4$ 个点集子集的生成子图是 $K_1$ 和 $K_2$，即 $4$ 个结点和 $4$ 条边。</p>


<pre><code class="language-input2">10
FF1
FF
F7
F3
F1
F
7
3
1
</code></pre>


<pre><code class="language-output2">10 45 120 210 252 210 120 45 10 1
</code></pre>


<p>这是一个 $10$ 个点的完全图，即 $K_{10}$，这组样例满足子任务 $2$ 的限制。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_clique3.in</code>和 <code>ex_clique3.out</code>，这组样例满足子任务 $3$ 的限制。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_clique4.in</code>和 <code>ex_clique4.out</code>。</p>
<h2>数据范围</h2>
<p>对于所有数据， $2\leq n\leq 8000$ ，令 $m$ 为 $G$ 中边数，则 $0\leq m\leq \frac{n(n-1)}{2}$，保证输入的 $G$ 是“优美”的。 </p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\leq$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$1000$</td>
<td style="text-align:center;">$m=\frac{n(n-1)}{2}$</td>
<td>$5$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">A</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$m\geq \frac{n(n-1)}{2}-20$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">无</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$4000$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$8000$</td>
<td style="text-align:center;">$30$</td>
</tr>
</tbody>
</table>
</div>
<p>特殊性质 A: $G$ 是一个完全 $k$ 分图，即 $\exists 1\leq k\leq n$ ，使 $G$ 点集可以被划分为 $k$ 个非空集合，两个点之间有边当且仅当它们不在同一集合中。</p>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>提示</h2>
<p><strong>请选手相信自己算法的常数与评测机的效率</strong>。</p>
<h2>下载</h2>
<p><a href="./21033/file/attachment.zip">样例数据下载</a></p>
