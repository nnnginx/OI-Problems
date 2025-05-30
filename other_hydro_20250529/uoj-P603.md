<p>众所周知，小葱同学擅长计算，尤其擅长计算组合数。但是对组合数有了充分研究的小葱同学对组合数失去了兴趣，而开始研究数列。</p>
<p>我们定义 $F_0 = a$，$F_1 = b$，$F_i = (F_{i-1} + F_{i-2}) \bmod m$（$i \ge 2$）。</p>
<p>现在给定 $n$ 组询问，对于每组询问请找到一个最小的整数 $p$，使得 $F_p = 0$。</p>
<h2>输入格式</h2>
<p>第一行两个整数 $n, m$，代表询问的组数和每组计算中的模数。</p>
<p>接下来 $n$ 行每行两个整数 $a, b$，代表一组询问中 $F_0$ 和 $F_1$ 的值。</p>
<h2>输出格式</h2>
<p>对于每组询问，输出一行一个整数 $p$ 代表答案。如果这样的 $p$ 不存在，输出 <code>-1</code>。</p>


<pre><code class="language-input1">4 5
0 1
1 2
2 3
3 4
</code></pre>


<pre><code class="language-output1">0
3
2
-1
</code></pre>



<pre><code class="language-input2">1 6
4 4
</code></pre>


<pre><code class="language-output2">3
</code></pre>


<h2>样例三</h2>
<p>见附加文件中 <code>ex_fib3.in</code> 与 <code>ex_fib3.ans</code>。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_fib4.in</code> 与 <code>ex_fib4.ans</code>。</p>
<h2>限制与约定</h2>
<p>对于所有测试点：$1 \le n, m \le {10}^5$，$0 \le a, b &lt; m$。</p>
<p>每个测试点的具体限制见下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n, m \le$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$3 \sim 4$</td>
<td style="text-align:center;" rowspan="3">${10}^5$</td>
<td style="text-align:center;">$m$ 是质数</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 6$</td>
<td style="text-align:center;">$m = p_1 p_2 \cdots p_k$，其中 $p_i$ 是两两不同的质数</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 10$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21007/file/attachment.zip">样例数据下载</a></p>
