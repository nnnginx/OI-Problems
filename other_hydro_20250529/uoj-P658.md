<p>跳蚤国王的密码本是一个长为 $n$，字符集为 $\{0, \dots, p-1\}$ 的字符串。跳蚤国王考虑了一种简单的哈希算法，取底数为 $b$，字符串 $\mathbf{s}=s_0s_1\dots s_{n-1}$ 的哈希值就是 $H(\mathbf{s}, b)=\sum_{i=0}^{n-1} s_i b^i \bmod p$。接着，跳蚤国王随机生成了一个字符串 $\mathbf{s}$，并选取了数 $q$，带入哈希函数验证了 $b=1,q,\dots,q^{n-1}$ 的这些情况。经过计算之后，跳蚤国王惊讶地发现仅对于 $k$ 个 $i$，$b=q^i$ 时的字符串哈希值不为 $0$。</p>
<p>这个消息被 Skip 蚤知道了，并且它已经窃取到了 $p, q, n$ 和这 $k$ 组 $(i, H(\mathbf{s}, q^i))$ 的值。此外，它还得知 $s_m$ 就是跳蚤国王的电脑登录密码。现在 Skip 蚤需要还原出 $s_m$ 的值。</p>
<p>这样，它就可以潜入 UOJ 服务器并把自己的 rating 改为 $8000$ ，并让跳蚤国王无法登陆电脑改回来了。</p>
<p>本题取 $p=998244353$，且保证 $1,q,\dots,q^{n-1}$ 在 $\bmod p$ 下是互不相同的，可以证明此时 $s_m$ 被唯一确定。</p>
<h2>输入格式</h2>
<p>第一行输入四个整数 $n, m, k, q$。分别表示字符串的长度，询问字符串位置，非零哈希值数量，以及所选的底数公比。</p>
<p>接下来 $k$ 行每行两个整数 $i, v$ 表示 $H(\mathbf{s}, q^i) = v$。</p>
<h2>输出格式</h2>
<p>输出一个数 $s_m$。</p>


<pre><code class="language-input1">3 0 3 10
0 6
1 123
2 10203
</code></pre>


<pre><code class="language-output1">3
</code></pre>


<p>不难验证 $\mathbf{s} = \texttt{321}$。因此 $s_0=3$。</p>


<pre><code class="language-input2">2 0 2 998244352
0 132
1 666
</code></pre>


<pre><code class="language-output2">399
</code></pre>



<pre><code class="language-input3">2000 0 10 3
1 1
2 2
3 3
4 4
5 5
6 6
7 7
8 8
9 9
10 10
</code></pre>


<pre><code class="language-output3">19212461
</code></pre>

<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，保证 $1\le n\le p-1, 0\le m\le n-1, 1\le k\le \min(n, 10^5), 1\le q\le p-1, 0\le i\le n-1, 1\le v\le p-1$，且输入的 $i$ 互不相同，$1,q,\dots,q^{n-1}$ 在 $\bmod p$ 下互不相同。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">$k\le$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;" colspan="2">$2\times 10^3$</td>
<td style="text-align:center;" rowspan="6">无</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$10^6$</td>
<td style="text-align:center;" rowspan="3">$1$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$10^7$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$p-1$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$10^6$</td>
<td style="text-align:center;" rowspan="3">$10^5$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$10^7$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;" rowspan="3">$p-1$</td>
<td style="text-align:center;">$q^n=1$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$2\times 10^3$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$3\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./21059/file/attachment.zip">样例数据下载</a></p>
