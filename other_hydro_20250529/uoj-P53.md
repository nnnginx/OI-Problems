<p>在元旦激光炮的轰炸下，圣诞老人终于招架不住仓皇而逃，元旦三侠立刻展开追击行动。</p>
<p>有 $n$ 座城市，之间有 $n - 1$ 条道路连接成一个树形结构。每个城市有一个停留时间 $w_i$，只要圣诞老人来到 $i$ 号城市就必须停留 $w_i$ 的时间休息一下。</p>
<p>圣诞老人的逃跑路线可以用长度 $l$ 的序列 $s_1, s_2, \dots, s_l$ 表示（$l$ 是某个正整数），他会依次飞过 $s_1, s_2, \dots, s_l$ 号城市然后飞向火星找楼主聊人生，耗费的时间为经过的城市的停留时间之和，即 $\sum_{i = 1}^l w_{s_i}$。（圣诞老人可能经过同一个城市多次）</p>
<p>由于元旦三侠身手敏捷，圣诞老人在城市 $i$ 的时候下一步能飞到的城市是受限制的。对于每个城市 $i$ 有三个整数参数 $a_i, b_i, c_i$ （$1 \leq a_i, b_i, c_i \leq n$）。从城市 $i$ 出发能飞到城市 $j$ 当且仅当<strong>下面三个条件中有至少一个成立</strong>：</p>
<ul><li>从城市 $a_i$ 出发沿道路行走到城市 $b_i$ 必经过城市 $j$。</li>
<li>从城市 $b_i$ 出发沿道路行走到城市 $c_i$ 必经过城市 $j$。</li>
<li>从城市 $c_i$ 出发沿道路行走到城市 $a_i$ 必经过城市 $j$。</li>
</ul><p>所以圣诞老人的长度为 $l$ 的逃跑路线 $s$ 必须满足对于所有的 $1 \leq i &lt; l$ 能从 $s_i$ 出发飞到 $s_{i + 1}$。</p>
<p>由于圣诞老人在和元旦三侠玩心理战，他会选择耗费时间前 $k$ 小的逃跑路线之一（长度 $l$ 不限）。请帮助元旦三侠找出耗费时间前 $k$ 小的逃跑路线的耗费时间吧。</p>
<p>由于世界被圣诞老人毁灭得差不多了，元旦三侠手上的电脑只有 $100\texttt{MB}$内存。<strong>请节约使用内存。</strong>测评机是 64 位机，指针类型和 <code>long</code> 类型均为 $8$ 个字节。</p>
<p>消灭圣诞老人！地球属于人类！</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n, k$。</p>
<p>第二行 $n$ 个整数，第 $i$ 个整数表示 $w_i$。保证 $1 \leq w_i \leq 10^8$。</p>
<p>第三行 $n - 1$ 个整数，第 $i$ 个整数即 $p_{i + 1}$ 表示 $i + 1$ 号城市与 $p_{i+1}$ 号城市之间有道路连接。保证 $1 \leq p_{i + 1} &lt; i + 1$。</p>
<p>接下来 $n$ 行，第 $i$ 行包含三个整数 $a_i, b_i, c_i$。保证 $1 \leq a_i, b_i, c_i \leq n$。</p>
<h2>输出格式</h2>
<p>$k$ 行，每行一个整数，第 $i$ 行表示第 $i$ 小的逃跑路线的耗费时间。</p>


<pre><code class="language-input1">4 9
1 10 15 1000
1 2 2
2 2 4
2 2 3
1 3 4
3 3 4
</code></pre>


<pre><code class="language-output1">1
10
11
15
16
20
21
25
25
</code></pre>

<h2>样例二</h2>
<p>见样例数据下载。这组样例满足 $a_i = b_i$。</p>
<h2>样例三</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$n$</th>
<th>$k$</th>
</tr></thead><tbody><tr><td>1, 2</td><td>$n = 5$</td><td>$k = 10$</td></tr><tr><td>3, 4</td><td>$n = 100$</td><td>$k = 100$</td></tr><tr><td>5, 6</td><td>$n = 1000$</td><td>$k = 50000$</td></tr><tr><td>7, 8</td><td>$n = 1000$</td><td>$k = 10^5$</td></tr><tr><td>9, 10</td><td>$n = 15000$</td><td>$k = 10^5$</td></tr><tr><td>11, 12</td><td>$n = 20000$</td><td>$k = 10^5$</td></tr><tr><td>13, 14</td><td>$n = 10^5$</td><td>$k = 10^5$</td></tr><tr><td>15, 16</td><td>$n = 10^5$</td><td>$k = 5 \times 10^5$</td></tr><tr><td>17, 18</td><td>$n = 5 \times 10^5$</td><td>$k = 10^5$</td></tr><tr><td>19, 20</td><td>$n = 5 \times 10^5$</td><td>$k = 5 \times 10^5$</td></tr></tbody></table></div>

<p>对于所有编号为奇数的测试点，输入中所有 $a_i = b_i$。</p>
<p>保证答案小于等于 $10^8$。</p>
<p><strong>时间限制：</strong>$3\texttt{s}$</p>
<p><strong>空间限制：</strong>$100\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20493/file/attachment.zip">样例数据下载</a></p>
