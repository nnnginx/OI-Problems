<p>UOI 终于考完了，现在你要以标准的宇宙通用语请获奖选手上台领奖。</p>
<p>现在邀请的这一批选手一共有 $n$ 个“人”。更准确地说，他们是一群脑回路几乎相同的外星蜜蜂，故而在比赛中取得了完全相同的分数。</p>
<p>宇宙通用语非常强大，一共有 $m$ 种符号。用这种语言表达每只外星蜜蜂的名字要么只需要一个符号，要么只需要两个符号。</p>
<p>你需要给这一批选手编写一份由他们所有人名字组成的获奖名单，再按顺序念出来。你可以做如下调整：</p>
<ol>
<li>你可以调整这 $n$ 个名字的排列顺序；</li>
<li>由于外星蜜蜂的特殊文化，所有两个符号的名字无论你顺着念还是倒着念，指代的都是同一只蜜蜂。所以名单中每个两个符号的名字你既可以按顺序写也可以按逆序写。</li>
<li>可能存在名字相同的多只蜜蜂，但你仍然要读这个名字多次。</li>
</ol>
<p>为了避免倾向性，你希望最后把名字顺次连起来是个回文串。也就是说，你要让名字串起来后的符号序列从左到右读和从右往左读没有区别。</p>
<p><strong>测试数据保证有解。</strong></p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n,m$，分别表示选手个数和符号数。选手从 $1 \ldots n$ 编号。</p>
<p>接下来 $n$ 行，第 $i$ 行先输入一个正整数 $l_i \in \{1,2\}$ 表示 $i$ 号选手的名字长度，下面 $l_i$ 个 $1 \sim m$ 间的整数，表示第 $i$ 个人的名字。</p>
<h2>输出格式</h2>
<p>第一行输出由 $n$ 个 $1\sim n$ 的整数组成的排列，第 $i$ 个为 $p_i$，表示最后名单的第 $i$ 个选手是 $p_i$ 号选手。</p>
<p>下一行输出 $n$ 个 $01$ 整数，第 $i$ 个为 $0$ 表示 $p_i$ 号选手的名字正着写（与输入顺序一致），为 $1$ 表示倒着写。</p>
<p>注意，如果 $p_i$ 号选手名字长度为 $1$，你可以随便输出 $0$ 或 $1$。如果有多种合法的获奖名单，你可以任意输出一个。</p>


<pre><code class="language-input1">4 2
2 1 1
2 1 2
1 1
1 2
</code></pre>


<pre><code class="language-output1">4 1 3 2 
0 1 0 0
</code></pre>


<p>样例一输出对应的回文串是 $211112$。</p>


<pre><code class="language-input2">2 2
1 1
2 1 2
</code></pre>


<pre><code class="language-output2">1 2 
0 1
</code></pre>


<p>样例二输出对应的回文串是 $121$。</p>
<h2>样例三</h2>
<p>见附加文件中 <code>ex_namelist3.in</code> 与 <code>ex_namelist3.out</code>，该组样例满足子任务 5 的性质。</p>
<h2>样例四</h2>
<p>见附加文件中 <code>ex_namelist4.in</code> 与 <code>ex_namelist4.out</code>，该组样例满足子任务 6 的性质。</p>
<h2>样例五</h2>
<p>见附加文件中 <code>ex_namelist5.in</code> 与 <code>ex_namelist5.out</code>，该组样例满足子任务 5 的性质。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，$1\leq n,m\leq 5\times 10^5$。令 $L=\sum_{i=1}^{n} l_i$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n,m\le$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$20$</td>
<td style="text-align:center;">$20$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$5\times 10^5$</td>
<td style="text-align:center;">$l_i=2$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$3000$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;" rowspan="3">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="3">$5\times 10^5$</td>
<td style="text-align:center;">$L$ 为偶数</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$L$ 为奇数</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">无</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
