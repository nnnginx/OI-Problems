<p><strong> 由于某些原因本题仅支持 C++, C++11 语言的提交。 </strong></p>
<p>Khong 阿姨在组织一场有 $x$ 位选手参加的竞赛，她打算给每位选手<strong>一袋饼干</strong>。总共有 $k$ 种不同类型的饼干，编号为从 $0$ 到 $k - 1$。类型为 $i$（$0 \le i \le k - 1$）的每块饼干都有一个<strong>口味值</strong> $2^i$。在 Khong 阿姨的食品储藏室里，有 $a_i$（有可能为 $0$）块类型为 $i$ 的饼干。</p>
<p>对每种类型的饼干，Khong 阿姨在每个袋子都会装上 $0$ 或者多块。所有袋子里面类型为 $i$ 的饼干的总块数不能超过 $a_i$。一个袋子里面所有饼干的口味值的总和，被称为这袋饼干的<strong>总口味值</strong>。</p>
<p>请帮 Khong 阿姨算一下，究竟存在多少不同的 $y$ 值，使得她可以装出 $x$ 袋饼干，而且每袋饼干的总口味值都等于 $y$。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>biscuits.h</code> 头文件。</p>
<p>你需要实现以下函数：</p>
<pre><code class="sh_cpp">long long count_tastiness(long long x, std::vector&lt;long long&gt; a)</code></pre>
<ul><li>$x$：需要装的饼干袋的数量。</li>
<li>$a$：长度为 $k$ 的数组。对 $0 \le i \le k - 1$，$a_i$ 表示在食物储藏室里类型为 $i$ 的饼干数量。</li>
<li>此函数应当返回不同 $y$ 值的数目，使得阿姨可以装出 $x$ 袋饼干，且每袋饼干的总口味值都为 $y$。</li>
<li>此函数会被调用 $q$ 次（对于允许的 $q$ 值，详见约束条件和子任务部分）。每次调用应当被看成是独立的场景。</li>
</ul><h2>输入格式</h2>
<p>评测程序示例将读取如下格式的输入数据。第一行包含一个整数 $q$。接下来是 $q$ 对这样的两行：它们按照下面的格式来描述一个单独的场景：</p>
<ul><li>第一行：$k\ x$</li>
<li>第二行：$a_0\ a_1\ \ldots\ a_{k - 1}$</li>
</ul><h2>输出格式</h2>
<p>评测程序示例的输出结果的格式如下：</p>
<ul><li>第 $i$ 行（$1 \le i \le q$）：<code>count_tastiness</code> 对于输入数据中第 $i$ 个场景的返回值。</li>
</ul>

<pre><code class="language-input1">2
3 3
5 2 1
3 2
2 1 2
</code></pre>


<pre><code class="language-output1">5
6
</code></pre>


<p>对于第一组数据：
考虑以下调用：</p>
<pre><code class="sh_cpp">count_tastiness(3, [5, 2, 1])</code></pre>
<p>这意味着阿姨打算装 $3$ 袋饼干，而在食物储藏室里总共有 $3$ 种类型的饼干：
- $5$ 块类型为 $0$ 的饼干，每块的口味值为 $1$，
- $2$ 块类型为 $1$ 的饼干，每块的口味值为 $2$，
- $1$ 块类型为 $2$ 的饼干，其口味值为 $4$。</p>
<p>$y$ 能够取的值为 $[0,1,2,3,4]$。举例来说，为了装出总口味值均为 $3$ 的 $3$ 袋饼干，阿姨可以这样装：</p>
<ul><li>一袋饼干里有 $3$ 块类型为 $0$ 的饼干，以及</li>
<li>两袋饼干，其中各有一块类型为 $0$ 的饼干和一块类型为 $1$ 的饼干。</li>
</ul><p>由于总共有 $5$ 个可能的 $y$ 值，函数应当返回 $5$。</p>
<p><img src="https://img.uoj.ac/problem/567/567_ex1.png" alt="样例一" class="img-responsive center-block" style="width:500px;"></p>
<p>对于第二组数据：</p>
<p>考虑如下调用：</p>
<pre><code class="sh_cpp">count_tastiness(2, [2, 1, 2])</code></pre>
<p>这意味着阿姨打算装 $2$ 袋饼干，而在食物储藏室里总共有 $3$ 种类型的饼干：
- $2$ 块类型为 $0$ 的饼干，每块的口味值为 $1$，
- $1$ 块类型为 $1$ 的饼干，其口味值为 $2$，
- $2$ 块类型为 $2$ 的饼干，每块的口味值为 $4$。</p>
<p>$y$ 能够取的值为 $[0,1,2,4,5,6]$，由于总共有 $6$ 个可能的 $y$ 值，函数应当返回 $6$。</p>
<h2>限制与约定</h2>
<p>对于全部数据，满足：</p>
<ul><li>$1\le k\le 60$</li>
<li>$1\le q\le 1000$</li>
<li>$1\le x\le 10^{18}$</li>
<li>$0\le a_i\le 10^{18}$（对于所有的 $0\le i\le k-1$）</li>
<li>对于 <code>count_tastiness</code> 的每次调用，食物储藏室里所有饼干的口味值总和都不会超过 $10^{18}$。</li>
</ul><p>详细子任务分值与附加限制如下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th style="text-align:center;">子任务</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
</tr></thead><tbody><tr><td style="text-align:center;">$1$</td>
<td style="text-align:center;">$q\le 10$，且对于 <code>count_tastiness</code> 的每次调用，食物储藏室里所有饼干的口味值总和都不会超过 $100\ 000$。</td>
<td style="text-align:center;">$9$</td>
</tr><tr><td style="text-align:center;">$2$</td>
<td style="text-align:center;">$x=1,q\le 10$</td>
<td style="text-align:center;">$12$</td>
</tr><tr><td style="text-align:center;">$3$</td>
<td style="text-align:center;">$x\le 10\ 000,q\le 10$</td>
<td style="text-align:center;">$21$</td>
</tr><tr><td style="text-align:center;">$4$</td>
<td style="text-align:center;">对于 <code>count_tastiness</code> 的每次调用，正确的返回结果都不会超过 $200\ 000$。</td>
<td style="text-align:center;">$35$</td>
</tr><tr><td style="text-align:center;">$5$</td>
<td style="text-align:center;">没有附加限制条件。</td>
<td style="text-align:center;">$23$</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$1 \texttt{s}$</p>
<p><strong>空间限制</strong>：$1024 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20971/file/attachment.zip">样例及测评库下载</a></p>
