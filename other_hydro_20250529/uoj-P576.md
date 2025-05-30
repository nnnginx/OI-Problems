<p>在大漠中奔波数周修好电站之后，你以迅雷不及掩耳之势在三天内搭好了“跳找”的基本框架。</p>
<p>现在你开始思考“跳找”服务器的部署和联动问题。</p>
<p>“跳找”计划布置 $n$ 个服务器，编号 $1\sim n$。</p>
<p>这 $n$ 个服务器被 $n-1$ 条网络线路连接，即线路形成一个树形结构。树以 $1$ 号服务器为根。</p>
<p>每个服务器 $u$ 都有一个组别 $val_u$，组别有 $m$ 个，分别为 $1\sim m$。</p>
<p>每条网络线路都有一定的延时，定义 $dis(u, v)$ 为服务器 $u, v$ 之间线路延时的和，即树上 $u,v$ 间简单路径的边权和。</p>
<p>定义服务器 $u$ 的延时为 $\sum\limits_{k=1}^m\max\limits_{val_v=k}dis(u,v)$，也即对每个组别的最大延迟求和。</p>
<p>为了测试整个服务器网络的性能，需要完成下列 $q$ 个操作：</p>
<ul>
<li><p>修改服务器 $u$ 的组别；</p>
</li>
<li><p>查询 $u$ 子树内所有服务器的延时总和。</p>
</li>
</ul>
<h2>输入格式</h2>
<p>第一行一共三个正整数 $n, m, q$，表示服务器个数，组别数以及操作个数。</p>
<p>第二行一行 $n$ 个数，第 $i$ 个数 $val_i$ 表示服务器 $i$ 一开始的组别。</p>
<p>第三行一行 $n - 1$ 个数，第 $i$ 个数 ${fa}_{i+1}$ 表示服务器 $i + 1$ 的父亲的编号。</p>
<p>第四行一行 $n - 1$ 个数，第 $i$ 个数 $len_{i+1}$ 表示服务器 $i + 1$ 与父亲之间的边的边长。</p>
<p>下面 $q$ 行，每行开头为一个正整数 $opt_i$，表示第 $i$ 次的操作类型：</p>
<ul>
<li><p>若 $opt_i = 1$，那么下面紧跟两个整数 $u_i, v_i$，表示将服务器 $u_i$ 的组别修改为 $v_i$；</p>
</li>
<li><p>若 $opt_i = 2$，后跟一个整数 $u_i$，表示查询 $u_i$ 子树内所有服务器的延时总和。</p>
</li>
</ul>
<p>保证一开始及每次操作过后，每个组别都拥有至少一个服务器。</p>
<h2>输出格式</h2>
<p>对于每个询问，输出一行一个整数，表示该询问的答案。</p>


<pre><code class="language-input1">8 3 6
1 2 3 2 3 2 2 3
1 2 2 1 5 6 4
1 1 1 1 1 1 1
2 1
2 2
1 4 1
2 5
1 7 3
2 2
</code></pre>


<pre><code class="language-output1">79
40
36
44
</code></pre>


<p>样例一中，每个服务器的延时如图 :</p>
<p><img src="https://img.uoj.ac/problem/576/coltree.png" alt="样例一" class="img-responsive center-block"></p>


<pre><code class="language-input2">15 4 5
2 1 3 4 1 3 3 4 2 1 2 2 1 3 2
1 1 3 2 2 1 3 4 9 10 4 8 12 10
60 39 99 85 78 41 87 70 19 8 60 60 18 3
2 1
2 2
2 3
2 4
2 5
</code></pre>


<pre><code class="language-output2">16657
3820
11041
8125
1396
</code></pre>



<pre><code class="language-input3">15 4 10
4 2 4 3 2 1 4 1 1 1 2 2 3 3 3 
1 1 3 3 4 2 7 8 7 6 11 9 11 6 
41 43 67 66 77 76 85 90 76 39 20 56 88 100 
1 12 1
2 1
1 7 1
2 1
1 1 1
2 1
1 13 2
2 1
1 4 2
2 1
</code></pre>


<pre><code class="language-output3">23399
22389
22045
21816
21816
</code></pre>

<h2>限制与约定</h2>
<p>对于所有的数据，保证 $1 \leq n, q\leq 2\times10^5,\ 2m\leq n\ ,1\leq len_i\leq 200, 1 \leq fa_i \lt i, 1 \leq u_i \leq n, 1 \leq v_i,val_i \leq m$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">$n,q\leq$</th>
<th style="text-align:center;">特殊性质</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$200$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$2000$</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$2\times 10^5$</td>
<td style="text-align:center;">不存在修改操作</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;" rowspan="2">$10^5$</td>
<td style="text-align:center;">询问操作中 $u_i=1$</td>
<td style="text-align:center;">$25$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;" rowspan="2">无</td>
<td style="text-align:center;">$15$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$2\times 10^5$</td>
<td style="text-align:center;">$20$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20980/file/attachment.zip">样例数据下载</a></p>
