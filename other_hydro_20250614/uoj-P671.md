<p>UOI 虽然非常高级，在赛时就可以得到成绩。但是在比赛结束的一刹那，一条外星亖手蚯蚓钻进了存储着比赛成绩的机器里，随即机器开始冒烟。</p>
<p>外星亖手蚯蚓立刻被众人控制住了，勒令将比赛成绩从该机器的数据盘里恢复出来。可是亖手蚯蚓脑回路比较奇怪，所以恢复数据的方式也非常的怪。</p>
<p>在一开始，数据盘里面存储着一个整数序列 $a$。然后每一步，亖手蚯蚓会先给定一个区间 $[l, r] (1 \leq l \leq r \leq n)$。然后进行以下三种操作之一：</p>
<ul>
<li><p>$1\ l\ r\ v$: 给定 $v$, 对于 $l \leq i \leq r$，将 $a_i$ 变为 $\lfloor \frac{a_i}{v} \rfloor$。这里我们保证 $v \ge 1$。</p>
</li>
<li><p>$2\ l\ r\ v$: 给定 $v$, 对于 $l \leq i \leq r$，将 $a_i$ 变为 $a_i \&amp; v$，其中 $\&amp;$ 是按位与运算。</p>
</li>
<li><p>$3\ l\ r$: 向你询问 $a_i$（$l \leq i \leq r$）的总和。</p>
</li>
</ul>
<p>虽然你不太理解亖手蚯蚓这通诡异的操作，但你还是乖乖地回答着亖手蚯蚓的一个个询问。不过有没有可能做得快一点呢？</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n, q$，表示序列 $a$ 的长度和询问个数。</p>
<p>下面一行 $n$ 个整数 $a_i$，<strong>以 $16$ 进制读入</strong>。</p>
<p>下面 $q$ 行，每行第一个正整数 $op_i$ 表示操作编号。</p>
<p>对于 $op_i = 1$ 或 $op_i = 2$，后面紧跟三个整数 $l_i, r_i, v_i$，表示执行上述对应操作, <strong>其中 $v_i$ 以 $16$ 进制读入</strong>。</p>
<p>对于 $op_i = 3$，后面紧跟两个整数 $l_i, r_i$，表示询问这个区间的元素的和对 $2^{128}$ 取模的值，<strong>以 $16$ 进制输出</strong>。</p>
<p>在本题中所有的十六进制数 <strong> 仅包含字符 <code>0</code> $\sim$ <code>9</code>,<code>a</code> $\sim$ <code>f</code>，分别代表着 $0 \sim 9,10 \sim 15$</strong>，同时 <strong>不存在无效前导零</strong> 。本题的所有 $16$ 进制输入保证满足如上格式，选手的输出也需要满足如上格式。</p>
<p><strong>提示: UOJ 中可以使用 $128$ 位无符号整型数字 <code>__uint128_t</code>，但需要手动实现 IO，我们提供了 IO 模板在题面结尾。</strong></p>
<h2>输出格式</h2>
<p>若干行，对于每个询问，输出其答案。</p>


<pre><code class="language-input1">5 5
1 9 1 9 1
3 2 3
2 1 3 5
3 1 5
1 1 5 3
3 1 5
</code></pre>


<pre><code class="language-output1">a
d
3
</code></pre>

<h2>样例二</h2>
<p>见附加文件中 <code>ex_machine2.in</code> 与 <code>ex_machine2.out</code>。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_machine3.in</code> 与 <code>ex_machine3.out</code>，其中所有数不超过 $2^{40}$。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1 \leq l_i \leq r_i \leq n \leq 300000, 1 \leq q \leq 200000, 0 \leq v_i, a_i \lt 2^{128}$，其中操作一的 $v_i \geq 1$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n\le$</th>
<th style="text-align:center;">$q\le$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;" rowspan="4">$3\times 10^5$ </td>
<td style="text-align:center;" rowspan="4">$2\times 10^5$</td>
<td style="text-align:center;">$op_i \neq 2$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$l_i = 1, r_i = n$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$op_i \neq 1$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$25$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{3s}$</strong></p>
<p><strong>空间限制：$\texttt{1GB}$</strong></p>
<h2>提示</h2>
<p><strong>提示：请注意你的算法的时间复杂度。</strong></p>
<p><strong>提示: UOJ 中可以使用 $128$ 位无符号整型数字 <code>__uint128_t</code>，但需要手动实现 IO，我们在下方提供了模板。</strong></p>
<pre><code class="sh_cpp">typedef __uint128_t u128;
inline u128 read() {
    static char buf[100];
    scanf("%s", buf);
    // std::cin &gt;&gt; buf;
    u128 res = 0;
    for(int i = 0;buf[i];++i) {
        res = res &lt;&lt; 4 | (buf[i] &lt;= '9' ? buf[i] - '0' : buf[i] - 'a' + 10);
    }
    return res;
}
inline void output(u128 res) {
    if(res &gt;= 16)
        output(res / 16);
    putchar(res % 16 &gt;= 10 ? 'a' + res % 16 - 10 : '0' + res % 16);
    //std::cout.put(res % 16 &gt;= 10 ? 'a' + res % 16 - 10 : '0' + res % 16);
}</code></pre>
