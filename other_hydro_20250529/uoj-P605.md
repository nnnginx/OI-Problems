<p>作为文化课大师，skip 蚤的大脑中组织着一份复杂的知识网络。</p>
<p>skip 蚤的知识网络中有 $n$ 个知识点，不妨将它们从 $1$ 至 $n$ 编号。skip 蚤在刷题历程中遇见过 $m$ 道令其印象深刻的习题，其中第 $i$ 道题在知识点 $u_i$ 和 $v_i$ 之间建立了联系。同时，每个知识点恰有一个标签，为了知识整理的便捷，标签的数量不会很多，只有 $k$ 个，不妨从 $1$ 至 $k$ 将它们编号。</p>
<p>知识网络帮助 skip 蚤从一个知识点快速发散思考到其他的知识点。定义<strong>思考序列</strong>为一个由知识点构成的序列 $a_1,a_2,\cdots,a_r$，满足对于所有 $1 \leq i \leq r-1$，要么知识点 $a_i$ 与 $a_{i+1}$ 之间建立了联系，要么知识点 $a_i$ 与 $a_{i+1}$ 拥有相同的标签。</p>
<p>为了考察发散思考的便捷程度，skip 蚤对两个不同的知识点 $1 \leq p &lt; q \leq n$ 定义知识网络上 $p,q$ 的<strong>思考便捷值</strong> $f(p,q)$ 为满足序列起始为 $p$、末尾为 $q$ 的思考序列的最短长度，如果不存在这样的序列，则 $f(p,q)=2k+1$。</p>
<p>skip 蚤想知道：对于 $1 \leq x \leq 2k+1$，有多少个二元组 $(p,q)(1 \leq p &lt; q \leq n)$ 满足 $f(p,q)=x$？</p>
<h2>输入格式</h2>
<p>第一行三个整数 $n,m,k$，分别表示知识网络中的知识点数、联系数和标签数。</p>
<p>第二行 $n$ 个整数 $p_1,p_2,\cdots,p_n$，其中 $p_i$ 表示编号为 $i$ 的知识点拥有的标签编号。</p>
<p>接下来 $m$ 行每行两个整数 $u_i,v_i$，表示在知识网络中知识点 $u_i$ 与知识点 $v_i$ 之间建立了联系。</p>
<h2>输出格式</h2>
<p>输出一行 $2k+1$ 个数，第 $i$ 个数表示有多少个二元组 $(p,q)(1 \leq p &lt; q \leq n)$ 满足 $f(p,q) = i$。</p>


<pre><code class="language-input1">6 3 3
1 2 2 3 3 3
3 4
4 5
4 3
</code></pre>


<pre><code class="language-output1">0 5 3 2 0 0 5
</code></pre>


<p>$f(2,3)=f(3,4)=f(4,5)=f(5,6)=f(4,6)=2$</p>
<p>$f(2,4)=f(3,5)=f(3,6)=3$</p>
<p>$f(2,5)=f(2,6)=4$</p>
<p>$f(1,2)=f(1,3)=f(1,4)=f(1,5)=f(1,6)=7$</p>
<h2>样例二</h2>
<p>见附加文件中 <code>ex_knowledge2.in</code> 与 <code>ex_knowledge2.out</code>，该组样例满足 $n,m \leq 3000$。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_knowledge3.in</code> 与 <code>ex_knowledge3.out</code>，该组样例无特殊性质。</p>
<h2>数据范围</h2>
<p>对于 $100\%$ 的数据，$1 \leq n \leq 5 \times 10^4 , 0 \leq m \leq 5 \times 10^4 , 1 \leq k \leq 150 , 1 \leq p_i \leq k , 1 \leq u_i,v_i \leq n, u_i \neq v_i$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">特殊性质</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$n \leq 500$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="2">$n,m \leq 3000$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;" rowspan="2">$m \leq 3000$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;" rowspan="2">$n,m \leq 2 \times 10^4,k \leq 60$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$k=10$,序列 $p$ 中每种数出现次数相同</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;" rowspan="2">无</td>
</tr>
<tr>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$4\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21009/file/attachment.zip">样例数据下载</a></p>
