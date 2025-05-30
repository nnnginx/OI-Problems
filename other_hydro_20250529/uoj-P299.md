<p>小 R 和室友小 B 在寝室里玩游戏。他们一共玩了 $n$ 局游戏，每局游戏的结果要么是小 R 获胜，要么是小 B 获胜。</p>
<p>第 $1$ 局游戏小 R 获胜的概率是 $p_1$，小 B 获胜的概率是 $1-p_1$。除了第一局游戏之外，每一局游戏小 R 获胜的概率与上一局游戏小 R 是否获胜有关。</p>
<p>具体来说：</p>
<ol><li>如果第 $i-1\ (1&lt; i\le n)$ 局游戏小 R 获胜，那么第 $i$ 局游戏小 R 获胜的概率为 $p_i$，小 B 获胜的概率为 $1-p_i$。</li>
<li>如果第 $i-1\ (1&lt; i\le n)$ 局游戏小 B 获胜，那么第 $i$ 局游戏小 R 获胜的概率为 $q_i$，小 B 获胜的概率为 $1-q_i$。</li>
</ol><p>小 D 时常过来看小 R 和小 B 玩游戏，因此他知道某几局游戏的结果。他想知道在他已知信息的条件下，小 R 在 $n$ 局游戏中获胜总局数的期望是多少。</p>
<p>小 D 记性不太好，有时他会回忆起某局游戏的结果，并把它加入到已知信息中；有时他会忘记之前某局游戏结果，并把它从已知信息中删除。你的任务是：每当小 D 在已知信息中增加或删除一条信息时，根据小 D 记得的已知信息，帮助小 D 计算小 R 在 $n$ 局游戏中获胜总局数的期望是多少。</p>
<p>需要注意的是：如果小 D 忘了一局游戏的结果，之后又重新记起，两次记忆中的游戏结果不一定是相同的。你不需要关心小 D 的记忆是否与实际情况相符，你只需要根据他的记忆计算相应的答案。</p>
<h2>输入格式</h2>
<p>第一行两个正整数 $n,m$ 和一个字符串 $type$。表示小 R 和小 B 一共玩了 $n$ 局游戏，小 D 一共进行了 $m$ 次修改已知信息的操作，该数据的类型为 $type$。$type$ 字符串是为了能让大家更方便地获得部分分，你可能不需要用到这个输入，其具体含义见<strong>限制与约定</strong>。</p>
<p>接下来 $n$ 行，第 $1$ 行包含一个实数 $p_1$，表示第一局比赛小R获胜的概率是 $p_1$。第 $i\ (1&lt; i \le n)$ 行包含两个实数 $p_i,q_i$。表示在第 $i-1$ 局游戏小 R 获胜的情况下，第 $i$ 局游戏小 R 获胜的概率是 $p_i$；$q_i$ 表示在第 $i-1$ 局游戏小 B 获胜的情况下，第 $i$ 局游戏小 R 获胜的概率是 $q_i$。</p>
<p>接下来 $m$ 行，每行描述一个小 D 已知信息的变化，操作分为两类。</p>
<ol><li><code>add i c</code> 表示小 D 回忆起了第 $i$ 局比赛的结果，并把它加入到已知信息中。若 $c=0$ 表示第 $i$ 局比赛小 B 获胜，若 $c=1$ 表示第 $i$ 局比赛小 R 获胜。数据保证 $i,c$ 均为整数且 $1\le i \le n,0\le c \le 1$，如果这个操作不是第一个操作，保证在上一个操作结束后的已知信息中没有第 $i$ 局比赛的结果。</li>
<li><code>del i</code> 表示小 D 忘记了第 $i$ 局比赛的结果，并把它从已知信息中删除。数据保证 $i$ 是整数且 $1\le i \le n$，保证在上一个操作结束后的已知信息中有第 $i$ 局比赛的结果。</li>
</ol><h2>输出格式</h2>
<p>对于每个操作，输出一行实数，表示操作结束后，在当前已知信息的条件下，小R在 $n$ 局游戏中总共获胜的局数的期望是多少。</p>


<pre><code class="language-input1">3 3 A
0.3
0.5 0.2
0.9 0.8
add 1 1
add 3 0
del 1
</code></pre>


<pre><code class="language-output1">2.350000
1.333333
0.432749
</code></pre>


<p>运用贝叶斯公式</p>
<h5>第一问</h5>
<p>$$p(x_2=1|x_1=1)=0.5,p(x_3=1|x_1=1)=0.5*0.9+0.5*0.8=0.85,E(x_1+x_2+x_3|x_1=1)=0.5+0.85+1=2.35$$</p>
<h5>第二问</h5>
<p>$$p(x_2=1|x_1=1,x_3=0)=\frac{p(x_3=0|x_1=1,x_2=1)p(x_2=1|x_3=0)}{p(x_3=0|x_1=1)} \approx 0.333,E(x_1+x_2+x_3|x_1=1,x_3=0) \approx 1.333$$</p>
<h5>第三问</h5>
<p>$$p(x_2=1|x_3=0)=\frac{p(x_3=0|x_2=1)p(x_2=1)}{p(x_3=0)}$$</p>
<p>其中</p>
<p>$$p(x_3=0|x_2=1)=0.1,p(x_2=1)=0.3*0.5+0.7*0.2=0.29,p(x_3=0)=0.29*0.1+0.71*0.2=0.171$$</p>
<p>所以 </p>
<p>$$p(x_2=1|x_3=0)=0.1*0.29/0.171 \approx 0.16959$$</p>
<p>$$p(x_1=1|x_3=0)=\frac{p(x_3=0|x_1=1)p(x_1=1)}{p(x_3=0)}$$</p>
<p>其中 </p>
<p>$$p(x_3=0|x_1=1)=0.5*0.1+0.5*0.2=0.15,p(x_1=1)=0.3,p(x_3=0)=0.171$$</p>
<p>所以 </p>
<p>$$p(x_1=1|x_3=0)=0.15*0.3/0.171 \approx 0.26316$$</p>
<p>$$E(x_1+x_2+x_3|x_3=0) \approx 0.43275$$</p>
<h2>样例二</h2>
<p>见样例数据下载。</p>
<h2>样例三</h2>
<p>见样例数据下载。</p>
<h2>评分标准</h2>
<p>如果你的答案与正确答案的绝对误差在 $10^{-4}$ 以内，则被判定为正确。</p>
<p>如果你的所有答案均为正确，则得满分，否则得 0 分。</p>
<p>请注意输出格式：每行输出一个答案，答案只能为一个实数。每行的长度不得超过 50。错误输出格式会被判定为 0 分。</p>
<h2>限制与约定</h2>
<p>对于100%的数据，$1\le n\le 200000, 1\le m \le 200000,0 &lt; p_i,q_i &lt; 1$。</p>
<p>对于100%的数据，<strong>输入保留最多四位小数</strong>。</p>
<p>本题共有20个数据点，每个数据点5分,每个测试点的具体约定如下表：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点</th>
<th>$n$</th>
<th>$m$</th>
<th>数据类型</th>
</tr></thead><tbody><tr><td>1-2</td><td>$\le 10$</td><td>$\le 20$</td><td>A</td></tr><tr><td>3-4</td><td>$\le 100$</td><td>$\le 100$</td><td>B</td></tr><tr><td>5-6</td><td>$\le 1000$</td><td>$\le 5000$</td><td>A</td></tr><tr><td>7-9</td><td>$\le 2000$</td><td>$\le 5000$</td><td>B</td></tr><tr><td>10-13</td><td>$\le 10000$</td><td>$\le 200000$</td><td>B</td></tr><tr><td>14-15</td><td rowspan="3">$\le 200000$</td><td rowspan="3">$\le 200000$</td><td>C</td></tr><tr><td>16-17</td><td>D</td></tr><tr><td>18-20</td><td>A</td></tr></tbody></table></div>

<p>数据类型的含义：</p>
<p>A：无限制</p>
<p>B：$\forall i &gt; 1,|p_i-q_i| &gt; 0.999$</p>
<p>C：同一时刻，小 D 最多只有 1 条已知信息</p>
<p>D：同一时刻，小 D 最多只有 5 条已知信息</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$512\texttt{MB}$</p>
<h2>小R教你学数学</h2>
<p>你<strong>可能</strong>会用到以下公式</p>
<ol><li><p>条件概率的计算方法</p>
<p>我们记 $p(A|B)$ 表示在已知事件 $B$ 发生时事件 $A$ 发生的概率，条件概率可以用以下公式计算：</p>
<p>$$p(A|B)=\frac{p(AB)}{p(B)}$$</p>
<p>其中$p(AB)$表示事件 $B$ 和事件 $A$ 同时发生的概率，$p(B)$ 表示事件 $B$ 发生的概率。</p>
</li>
<li><p>贝叶斯公式(Bayes)</p>
<p>由条件概率的计算方法，我们容易得到贝叶斯公式</p>
<p>$$p(A|B)=\frac{p(B|A)p(A)}{p(B)}$$</p>
</li>
<li><p>全概率公式</p>
<p>如果随机变量 $x$ 有 $k$ 个取值，分别为 $x_1,x_2,\ldots,x_k$ 那么</p>
<p>$$p(A)=\sum_{i=1}^k p(A|x=x_i)p(x=x_i)$$</p>
</li>
</ol><h2>温馨提示</h2>
<p>在本题中，如果你<strong>希望获得全部的分数</strong>，你<strong>可能</strong>需要考虑由于浮点数运算引入的误差。只使用加法和乘法运算不会引入太大的误差，但请谨慎使用减法和除法。</p>
<ol><li>两个大小相近的数相减可以引入非常大的相对误差。</li>
<li>如果一个矩阵的行列式值非常小，那么求解该矩阵的逆可以带来相当大的误差。</li>
</ol><p>当然，如果你的算法在数学上是正确的，但没有考虑浮点数运算的误差问题，可能仍然可以获得一部分的分数。</p>
<h2>下载</h2>
<p><a href="./20727/file/attachment.zip">样例数据下载</a></p>
