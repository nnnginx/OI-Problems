<p>今年夏天，NOI在SZ市迎来了她30周岁的生日。来自全国$n$城市的OIer们都会从各地出发，到SZ市参加这次盛会。</p>
<p>全国的城市构成了一棵以SZ市为根的有根树，每个城市与它的父亲用道路连接。为了方便起见，我们将全国的$n$个城市用 1 到$n$的整数编号。其中SZ市的编号为$1$。对于除SZ市之外的任意一个城市$v$,我们给出了它在这棵树上的父亲城市$f_v$以及到父亲城市道路的长度$s_v$。</p>
<p>从城市$v$前往SZ市的方法为：选择城市$v$的一个祖先$a$，支付购票的费用，乘坐交通工具到达$a$。再选择城市$a$的一个祖先$b$，支付费用并到达$b$。以此类推，直至到达SZ市。</p>
<p>对于任意一个城市$v$，我们会给出一个交通工具的距离限制$l_v$。对于城市$v$的祖先$a$，只有当它们之间所有道路的总长度不超过$l_v$时，从城市$v$才可以通过一次购票到达城市$a$，否则不能通过一次购票到达。对于每个城市$v$，我们还会给出两个非负整数$p_v,q_v$作为票价参数。若城市$v$到城市$a$所有道路的总长度为$d$，那么从城市$v$到城市$a$购买的票价为$dp_v+q_v$。</p>
<p>每个城市的OIer都希望自己到达SZ市时，用于购票的总资金最少。你的任务就是，告诉每个城市的OIer他们所花的最少资金是多少。</p>
<h2>输入格式</h2>
<p>输入文件的第1行包含2个非负整数$n,t$，分别表示城市的个数和数据类型（其意义将在后面提到）。
输入文件的第2到$n$行，每行描述一个除SZ之外的城市。其中第$v$行包含5个非负整数$f_v,s_v,p_v,q_v,l_v$，分别表示城市$v$的父亲城市，它到父亲城市道路的长度，票价的两个参数和距离限制。</p>
<p>请注意：<strong>输入不包含编号为1的SZ市，第2行到第n行分别描述的是城市2到城市n。</strong></p>
<h2>输出格式</h2>
<p>输出包含$n-1$行，每行包含一个整数。其中第$v$行表示从城市$v+1$出发，到达SZ市最少的购票费用。</p>
<p>同样请注意：<strong>输出不包含编号为1的SZ市。</strong></p>


<pre><code class="language-input1">7 3
1 2 20 0 3
1 5 10 100 5
2 4 10 10 10
2 9 1 100 10
3 5 20 100 10
4 4 20 0 10
</code></pre>


<pre><code class="language-output1">40
150
70
149
300
150
</code></pre>


<p>从每个城市出发到达SZ的路线如下（其中箭头表示一次直达）：</p>
<p>城市 2：只能选择 $2\rightarrow 1$，花费为$2\times 20+0=40$。</p>
<p>城市 3：只能选择 $3\rightarrow 1$，花费为$5\times 10+100=150$。</p>
<p>城市 4：由于 $4+2=6\le l_4=10$，故可以选择 $4\rightarrow 1$。若选择$4\rightarrow 1$，花费为$(4+2)\times 10+10=70$；若选择$4\rightarrow 2\rightarrow 1$，则花费为$(4\times 10+10)+(2\times 20+0)=90$；因此选择$4\rightarrow 1$。</p>
<p>城市 5：只能选择$5\rightarrow 2\rightarrow 1$，花费为$(9\times 1+100)+(2\times 20+0) = 149$；无法选择$5\rightarrow 1$，因为$l_5 = 10$，而城市5到城市1总路程为 $9 + 2 = 11 \gt l_5$，城市5不能直达城市 1。</p>
<p>城市 6：若选择$6\rightarrow 1$，花费为$(5+5)\times 20+100=300$；若选择$6\rightarrow 3\rightarrow 1$，花费为$(5\times 20+100)+(5\times 10+100)=350$；因此选择$6\rightarrow 1$。</p>
<p>城市 7：选择$7\rightarrow 4\rightarrow 1$，花费为$(4\times 20+0)+((4+2)\times 10+10)=150$；其他方案均比该方案差。</p>
<h2>样例二</h2>
<p>见样例数据下载。</p>
<p>该组样例按照城市编号几乎平均分为了4个部分，每个部分有不同的特点。你可以使用它们进行针对性的测试。</p>
<h2>限制与约定</h2>
<p>对于所有测试数据，保证$0 \leq p_v \leq 10^6$，$0 \leq q_v \leq 10^{12}$，$1 \leq f_v &lt; v$；保证$0 &lt; s_v \leq l_v \leq 2 \times 10^{11}$，且任意城市到SZ市的总路程长度不超过$2 \times 10^{11}$。</p>
<p>输入的$t$表示数据类型，$0 \leq t &lt; 4$，其中：</p>
<p>当$t = 0$或$2$时，对输入的所有城市$v$，都有 $f_v = v - 1$，即所有城市构成一个以SZ市为终点的链；</p>
<p>当$t = 0$或$1$时，对输入的所有城市$v$，都有 $l_v = 2 \times 10^{11}$，即没有移动的距离限制，每个城市都能到达它的所有祖先。</p>
<p>当$t = 3$时，数据没有特殊性质。</p>
<p>每组测试数据的$n$和$t$如下所示：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n$</th><th>$t$</th></tr></thead><tbody><tr><td>1</td><td>$n = 2 \times 10$</td><td>$t = 2$</td></tr><tr><td>2</td><td rowspan="2">$n = 2 \times 10^3$</td><td>$t = 0$</td></tr><tr><td>3</td><td>$t = 3$</td></tr><tr><td>4</td><td rowspan="7">$n = 2 \times 10^5$</td><td>$t = 0$</td></tr><tr><td>5</td><td>$t = 2$</td></tr><tr><td>6</td><td rowspan="3">$t = 1$</td></tr><tr><td>7</td></tr><tr><td>8</td></tr><tr><td>9</td><td rowspan="2">$t = 3$</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>时间限制：</strong>$3\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20447/file/attachment.zip">样例数据下载</a></p>
