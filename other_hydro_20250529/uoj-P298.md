<p>一个一般的网络系统可以被描述成一张无向连通图。图上的每个节点为一个服务器，连接服务器与服务器的数据线则看作图上的一条边，边权为该数据线的长度。两个服务器之间的通讯距离被定义为其对应节点之间最短路的长度。</p>
<p>现在，考虑一个当前图结构为树的网络系统。你作为该网络系统的管理员，被要求在这个系统中新加入一条给定长度的数据线。数据线可以连在任意两个服务器上。</p>
<p>你的任务是，求出在所有合法的方案中，通讯距离最远的两个服务器之间的最小距离。</p>
<h2>输入格式</h2>
<p>输入包含多组数据。对于每组数据，输入的第一行包含二个正整数 $N, L$, 其中 $N$表示服务器个数，$L$ 为新加入数据线的长度。</p>
<p>接下来 $n - 1$ 行，第 $i$ 行有三个正整数 $a_i, b_i, l_i$，表示有一条长度为 $l_i$ 的数据线连接服务器 $a_i, b_i$。服务器的编号为 $1 \sim N$。</p>
<p>输入的末尾以两个 $0$ 作为结束。</p>
<h2>输出格式</h2>
<p>对于每组数据，输出一行一个整数，描述在所有合法的方案中，通讯距离最远的两个服务器之间的最小距离。</p>


<pre><code class="language-input1">7 1
1 2 1
2 3 1
3 4 1
4 5 1
5 6 1
6 7 1
0 0
</code></pre>


<pre><code class="language-output1">3
</code></pre>



<pre><code class="language-input2">6 26
1 2 66
2 3 11
3 4 73
2 5 77
3 6 33
10 47
1 2 86
2 3 69
3 4 41
4 5 26
5 6 41
2 7 73
3 8 77
4 9 2
5 10 65
0 0
</code></pre>


<pre><code class="language-output2">143
232
</code></pre>

<h2>样例三</h2>
<p>见样例数据下载。</p>
<h2>限制与约定</h2>
<p>一共有 20 个测试点。编号为 $1 \sim 20$。每个测试点为 5 分。</p>
<p>保证在任一测试点中，数据的组数不会超过 $15$，且所有数据的 $N$ 之和不超过数据范围中标明的 $N$ 的最大值的 $5$ 倍。</p>
<p>保证所有的输入数据均为不超过 $2^{31}-1$ 的非负整数，保证 $N \geq 1$。</p>
<p>保证数据合法。</p>
<p>对于给定的测试点，其限制条件如下表所示。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点</th>
<th>$N$</th>
<th>测试点</th>
<th>$N$</th>
</tr></thead><tbody><tr><td>1</td><td>$\le 10$</td><td>11</td><td rowspan="5">$\le 20000$</td></tr><tr><td>2</td><td>$\le 50$</td><td>12</td></tr><tr><td>3</td><td rowspan="2">$\le 100$</td><td>13</td></tr><tr><td>4</td><td>14</td></tr><tr><td>5</td><td>$\le 150$</td><td>15</td></tr><tr><td>6</td><td rowspan="3">$\le 600$</td><td>16</td><td rowspan="5">$\le 100000$</td></tr><tr><td>7</td><td>17</td></tr><tr><td>8</td><td>18</td></tr><tr><td>9</td><td rowspan="2">$\le 2000$</td><td>19</td></tr><tr><td>10</td><td>20</td></tr></tbody></table></div>

<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20726/file/attachment.zip">样例数据下载</a></p>
