<p><em>追逐影子的人，自己就是影子。 ——荷马</em></p>
<p>Allison 最近迷上了文学。她喜欢在一个慵懒的午后，细细地品上一杯卡布奇诺，静静地阅读她爱不释手的《荷马史诗》。但是由《奥德赛》和《伊利亚特》组成的鸿篇巨制《荷马史诗》实在是太长了，Allison 想通过一种编码方式使得它变得短一些。</p>
<p>一部《荷马史诗》中有 $n$ 种不同的单词，从 $1$ 到 $n$ 进行编号。其中第 $i$ 种单词出现的总次数为 $w_i$。Allison 想要用 $k$ 进制串 $s_i$ 来替换第 $i$ 种单词，使得其满足如下要求:</p>
<p>对于任意的 $1 \leq i, j \leq n$，$i \neq j$，都有：$s_i$ 不是 $s_j$ 的前缀。</p>
<p>现在 Allison 想要知道，如何选择 $s_i$，才能使替换以后得到的新的《荷马史诗》长度最小。在确保总长度最小的情况下，Allison 还想知道最长的 $s_i$ 的最短长度是多少？</p>
<p>一个字符串被称为 $k$ 进制字符串，当且仅当它的每个字符是 $0$ 到 $k − 1$ 之间（包括 $0$ 和 $k − 1$）的整数。</p>
<p>字符串 $\mathrm{Str1}$ 被称为字符串 $\mathrm{Str2}$ 的前缀，当且仅当：存在 $1 \leq t \leq m$，使得 $\mathrm{Str1} = \mathrm{Str2}[1..t]$。其中，$m$ 是字符串 $\mathrm{Str2}$ 的长度，$\mathrm{Str2}[1..t]$ 表示 $\mathrm{Str2}$ 的前 $t$ 个字符组成的字符串。</p>
<h2>输入格式</h2>
<p>输入文件的第 $1$ 行包含 $2$ 个正整数 $n, k$，中间用单个空格隔开，表示共有 $n$ 种单词，需要使用 $k$ 进制字符串进行替换。</p>
<p>接下来 $n$ 行，第 $i + 1$ 行包含 $1$ 个非负整数 $w_i$，表示第 $i$ 种单词的出现次数。</p>
<h2>输出格式</h2>
<p>输出文件包括 2 行。</p>
<p>第 $1$ 行输出 $1$ 个整数，为《荷马史诗》经过重新编码以后的最短长度。</p>
<p>第 $2$ 行输出 $1$ 个整数，为保证最短总长度的情况下，最长字符串 $s_i$ 的最短长度。</p>


<pre><code class="language-input1">4 2
1
1
2
2
</code></pre>


<pre><code class="language-output1">12
2
</code></pre>


<p>用 $X_{(k)}$ 表示 $X$ 是以 $k$ 进制表示的字符串。</p>
<p>一种最优方案：令 $00_{(2)}$ 替换第 $1$ 种单词，$01_{(2)}$ 替换第 $2$ 种单词，$10_{(2)}$ 替换第 $3$ 种单词，$11_{(2)}$ 替换第 $4$ 种单词。在这种方案下，编码以后的最短长度为：</p>
<p>$1 \times 2 + 1 \times 2 + 2 \times 2 + 2 \times 2 = 12$</p>
<p>最长字符串 $s_i$ 的长度为 $2$。</p>
<p>一种非最优方案：令 $000_{(2)}$ 替换第 $1$ 种单词，$001_{(2)}$ 替换第 $2$ 种单词，$01_{(2)}$ 替换第 3 种单词，$1_{(2)}$ 替换第 $4$ 种单词。在这种方案下，编码以后的最短长度为：</p>
<p>$1 \times 3 + 1 \times 3 + 2 \times 2 + 2 \times 1 = 12$</p>
<p>最长字符串 $s_i$ 的长度为 $3$。与最优方案相比，文章的长度相同，但是最长字符串的长度更长一些。</p>


<pre><code class="language-input2">6 3
1
1
3
3
9
9
</code></pre>


<pre><code class="language-output2">36
3
</code></pre>


<p>一种最优方案：令 $000_{(3)}$ 替换第 $1$ 种单词，$001_{(3)}$ 替换第 $2$ 种单词，$01_{(3)}$ 替换第 $3$ 种单词，$02_{(3)}$ 替换第 $4$ 种单词，$1_{(3)}$ 替换第 $5$ 种单词，$2_{(3)}$ 替换第 $6$ 种单词。</p>
<h2>样例三</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th><th>$n$ 的规模</th><th>$k$ 的规模</th><th>备注</th><th>约定</th></tr></thead><tbody><tr><td>1</td><td>$n = 3$</td><td>$k = 2$</td><td></td><td rowspan="20">$0 &lt; w_i \leq 10^{11}$</td></tr><tr><td>2</td><td>$n = 5$</td><td>$k = 2$</td><td></td></tr><tr><td>3</td><td>$n = 16$</td><td>$k = 2$</td><td>所有 $w_i$ 均相等</td></tr><tr><td>4</td><td>$n = 1000$</td><td>$k = 2$</td><td>$w_i$ 在取值范围内均匀随机</td></tr><tr><td>5</td><td>$n = 1000$</td><td>$k = 2$</td><td></td></tr><tr><td>6</td><td>$n = 100000$</td><td>$k = 2$</td><td></td></tr><tr><td>7</td><td>$n = 100000$</td><td>$k = 2$</td><td>所有 $w_i$ 均相等</td></tr><tr><td>8</td><td>$n = 100000$</td><td>$k = 2$</td><td></td></tr><tr><td>9</td><td>$n = 7$</td><td>$k = 3$</td><td></td></tr><tr><td>10</td><td>$n = 16$</td><td>$k = 3$</td><td>所有 $w_i$ 均相等</td></tr><tr><td>11</td><td>$n = 1001$</td><td>$k = 3$</td><td>所有 $w_i$ 均相等</td></tr><tr><td>12</td><td>$n = 99999$</td><td>$k = 4$</td><td>所有 $w_i$ 均相等</td></tr><tr><td>13</td><td>$n = 100000$</td><td>$k = 4$</td><td></td></tr><tr><td>14</td><td>$n = 100000$</td><td>$k = 4$</td><td></td></tr><tr><td>15</td><td>$n = 1000$</td><td>$k = 5$</td><td></td></tr><tr><td>16</td><td>$n = 100000$</td><td>$k = 7$</td><td>$w_i$ 在取值范围内均匀随机</td></tr><tr><td>17</td><td>$n = 100000$</td><td>$k = 7$</td><td></td></tr><tr><td>18</td><td>$n = 100000$</td><td>$k = 8$</td><td>$w_i$ 在取值范围内均匀随机</td></tr><tr><td>19</td><td>$n = 100000$</td><td>$k = 9$</td><td></td></tr><tr><td>20</td><td>$n = 100000$</td><td>$k = 9$</td><td></td></tr></tbody></table></div>

<p>对于所有数据，保证 $2 \leq n \leq 100000$，$2 \leq k \leq 9$。</p>
<p><strong>选手请注意使用 64 位整数进行输入输出、存储和计算。</strong></p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
<h2>评分方式</h2>
<p>对于每个测试点：</p>
<p>若输出文件的第 $1$ 行正确，得到该测试点 40% 的分数；</p>
<p>若输出文件完全正确，得到该测试点 100% 的分数。</p>
<h2>下载</h2>
<p><a href="./20570/file/attachment.zip">样例数据下载</a></p>
