<p><strong>这是一道交互题。</strong></p>
<p>跳蚤国王发现通过后门破解密码，可能要等到 2050 年了。</p>
<p>因此，跳蚤国王觉得直接破解开机密码或许更为高效。</p>
<p>国王的密码可以被表示为一个神秘的 $n$ 阶矩阵 $A$，它的元素都是 $0\sim 998244352$ 之间的整数。</p>
<p>国王发现尽管无法直接获得开机密码。但是可以通过 Linux 跳蚤版的漏洞获得关于密码的信息。</p>
<p>具体来说，你可以向交互库进行若干次询问，每次给定交互库另一个元素都是 $0\sim 998244352$ 之间整数的 $n$ 阶矩阵 $B$，交互库会返回 $\det(A+B)$ 对 $998244353$ 取模的值。因为安全限制，你最多只能进行 $T$ 次询问。</p>
<p>你的任务是帮助国王猜测出原来的矩阵 $A$。 </p>
<p>这里 $\det(A)$ 表示方阵 $A$ 的行列式。</p>
<h2>任务</h2>
<p><strong>本题只支持C++。</strong></p>
<p>你必须引用 <code>password.h</code> 头文件。</p>
<p>你需要实现下面的过程：</p>
<pre><code class="sh_cpp">std::vector&lt;int&gt; solve(int n,int T);</code></pre>
<p>其中 $n$ 是矩阵 $A$ 的阶数，$T$ 是你最多的询问次数。你需要返回一个长度恰为 $n^2$ 的 <code>vector</code>，里面依次列出矩阵 $A$ 的所有元素，其中下标为 $(i-1)\times n+j-1$ 的位置为矩阵 $A$ 的 $(i,j)$ 位置元素 $A_{i,j}$。</p>
<p>你可以调用以下过程和交互库进行交互：</p>
<pre><code class="sh_cpp">int query(std::vector&lt;int&gt; vt);</code></pre>
<p>其中 <code>vt</code> 是一个长度恰为 $n^2$ 的 <code>vector</code>，里面依次列出你这次给定的矩阵 $B$ 的所有元素，其中下标为 $(i-1)\times n+j-1$ 的位置为矩阵 $B$ 的 $(i,j)$ 位置元素 $B_{i,j}$。交互库会返回 $\det(A+B)$ 对 $998244353$ 取模的值。你必须保证 <code>vt</code> 中所有元素都在 $0\sim 998244352$ 之间且长度为 $n^2$，不然交互库会返回 $-1$ 且你的交互过程会被判定为失败。你至多只能调用 $T$ 次 <code>query</code> 函数。</p>
<h2>评测方式</h2>
<p>样例评测库将读入如下格式的输入数据：</p>
<p>第一行包括两个正整数 $n$ 和 $T$，表示矩阵 $A$ 的阶数与你最多的询问次数。</p>
<p>接下来 $n$ 行，每行 $n$ 个整数，其中第 $i$ 行第 $j$ 个整数为矩阵 $A$ 的 $(i,j)$ 位置元素 $A_{i,j}$。</p>
<p><strong>在最终测试中，矩阵 $A$ 是确定的，不会因为你的询问而改变。</strong></p>
<p>样例评测库将输出如下格式的输出数据：</p>
<p>对于每一组数据，如果你正确猜测出了矩阵 $A$ 且询问次数没有超过限制次数，会输出你的询问次数 $cnt$，否则会输出 <code>Wrong Answer.</code>。</p>


<pre><code class="language-input1">1 1
2
</code></pre>


<pre><code class="language-output1">1
</code></pre>


<p>你可以直接调用 <code>query([0])</code> 来得到 $\det(A)$，由于 $n=1$，这正好也是 $A$ 的唯一一个元素。</p>
<h2>数据范围</h2>
<p>对于所有数据，$1\leq n\leq 50,1\leq T\leq 8000,0\leq A_{i,j}\leq 998244352$。</p>
<p>保证若你的交互过程满足题目限制，交互库不会占用超过 $0.5\texttt{s}$ 时间和 $32\texttt{MB}$ 内存。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">$T=$</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$5$</td>
<td>$14$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$4$</td>
<td>$6$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$8000$</td>
<td>$24$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$2501$</td>
<td>$27$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$50$</td>
<td style="text-align:center;">$2500$</td>
<td>$29$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21056/file/attachment.zip">样例数据与样例评测库下载</a></p>
