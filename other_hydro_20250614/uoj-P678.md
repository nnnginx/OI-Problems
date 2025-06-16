<p>小 R 有 $m$（$1 \le m \le 1000$）个机器人和 $m$ 张纸带，第 $i$（$1 \le i \le m$）个机器人负责对第 $i$ 张纸带进行操作。对于每张纸带，它们都被从左到右分成了 $n$（$1 \le n \le 32$）个格子，依次编号为 $0, 1, \ldots , n - 1$。每个格子有 $3$ 种状态：1. 格子上写有数字 $0$；2. 格子上写有数字 $1$；3. 格子是一个空格子。</p>
<p>在任意时刻，机器人<strong>必须</strong>站在纸带上的一个格子中。在设定好机器人在纸带上的初始位置后，第 $i$ 个机器人会依次执行预先设定的操作序列 $S_i$，操作由 <code>R</code>、<code>0</code>、<code>1</code>、<code>*</code> 四种字符组成，其中：</p>
<ol>
<li><code>R</code> 表示机器人向右走一格，如果右边没有格子，则机器人会原地爆炸；</li>
<li><code>0</code> 表示如果机器人所在格子非空，则将该格子上的数字改为 $0$，否则不修改；</li>
<li><code>1</code> 表示如果机器人所在格子非空，则将该格子上的数字改为 $1$，否则不修改；</li>
<li><code>*</code> 表示如果机器人所在格子非空，则将格子上的数字 $x$ 改为 $1 - x$，否则不修改。</li>
</ol>
<p>第 $i$ 张纸带的状态可以用一个长度为 $n$ 的序列表示，每个元素为 <code>0</code>、<code>1</code> 或 <code>-</code>（空格子），依次表示其每个格子的状态。第 $i$ 张纸带的初始状态称为机器人 $i$ 的输入 $X_i$，操作执行完成后纸带的状态称为机器人 $i$ 的输出 $Y_i$。注意，如果机器人爆炸了，那么这个机器人就没有输出。</p>
<p>可以发现，如果一个格子为空，那么机器人永远不会修改它。所以每个机器人都有如下特性：如果第 $i$ 个机器人所在的纸带上的<strong>所有格子</strong>都为空，那么它就不会执行任何操作，它的输出即为所有格子都为空。</p>
<p>现在小 R 给定了每一个机器人的输入 $X_i$（即每张纸带的初始状态）以及目标输出 $Y_i$。小 R 希望小 D 找到一个位置 $p$（$0 \le p &lt; n$），使得<strong>所有机器人</strong>都能以其所在纸带的第 $p$ 个格子为初始位置，在不爆炸的情况下执行完所有操作，并且满足第 $i$ 个机器人的输出为 $Y_i$。</p>
<p>小 D 花了几毫秒解决了问题，现在他想知道，有多少个输入和输出的组合方式使得上述问题有解，即有多少种为每个机器人设定输入 $X_0, X_1, \ldots , X_{m - 1}$ 和目标输出 $Y_0, Y_1, \ldots , Y_{m - 1}$ 的方式，使得至少存在一个位置 $p$（$0 \le p &lt; n$），使得所有机器人都能以其所在纸带的第 $p$ 个格子为起点，在不爆炸的情况下执行完所有操作，且满足第 $i$ 个机器人的输出为 $Y_i$。请你帮助小 D 解决这个问题，由于最终的答案可能很大，请你输出答案对 ${10}^9 + 7$ 取模后的余数。</p>
<p>两个组合方式不同当且仅当，存在至少一个机器人，它的输入或是目标输出在两个方式中不同。</p>
<h2>输入格式</h2>
<p>第一行包含两个正整数 $n, m$，分别表示每张纸带上的格子数和纸带数量。</p>
<p>接下来 $m$ 行，第 $i$ 行输入一个仅包含 <code>R</code> <code>0</code> <code>1</code> <code>*</code> 这四种字符的字符串 $S_i$，表示第 $i$ 个机器人的操作序列。</p>
<h2>输出格式</h2>
<p>仅一行一个正整数，表示答案模 ${10}^9 + 7$ 后的余数。</p>


<pre><code class="language-input1">2 1
1R*
</code></pre>


<pre><code class="language-output1">9
</code></pre>


<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">方案编号</th>
<th style="text-align:center;">输入 $X_0$</th>
<th style="text-align:center;">目标输出 $Y_0$</th>
<th style="text-align:center;">可行初始位置 $p$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;"><code>--</code></td>
<td style="text-align:center;"><code>--</code> </td>
<td style="text-align:center;">$0, 1$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;"><code>0-</code></td>
<td style="text-align:center;"><code>1-</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;"><code>1-</code></td>
<td style="text-align:center;"><code>1-</code> </td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;"><code>-0</code></td>
<td style="text-align:center;"><code>-1</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;"><code>-1</code></td>
<td style="text-align:center;"><code>-0</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;"><code>00</code></td>
<td style="text-align:center;"><code>11</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;"><code>10</code></td>
<td style="text-align:center;"><code>11</code> </td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;"><code>01</code></td>
<td style="text-align:center;"><code>10</code></td>
<td style="text-align:center;">$0$</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;"><code>11</code></td>
<td style="text-align:center;"><code>10</code> </td>
<td style="text-align:center;">$0$</td>
</tr>
</tbody>
</table>
</div>
<p>表中 <code>-</code> 表示空格子。注意方案 $1$ 的输入和输出中有两个空格子。</p>
<p>当输入全为空时，初始位置可以是 $0$ 或 $1$，因为根据题意，输入全为空时机器人不会执行任何操作。</p>
<p>当输入不全为空时，初始位置只能为 $0$，如果初始位置为 $1$ 机器人一定会爆炸。所以此时实际执行的操作是将第一格的数字改为 $1$，并将第二格的数字 $x$ 改为 $1 - x$。</p>


<pre><code class="language-input2">3 2
1R0
*
</code></pre>


<pre><code class="language-output2">1468
</code></pre>



<pre><code class="language-input2">3 2
1R0
*
</code></pre>


<pre><code class="language-output2">1468
</code></pre>


<p>可以用容斥原理来计算这个样例。</p>
<ol>
<li>初始位置 $p = 0$ 可以使得执行完所有操作后满足条件。那么第一个机器人的纸带 $0$ 号格子要么输入输出都是空，要么目标输出是 $1$（输入无所谓），所以有 $3$ 种方案；$1$ 号格子要么输入输出都是空，要么目标输出是 $0$，也是 $3$ 种方案；$2$ 号格子要么输入输出都是空，要么输入和目标输出相同（因为没有对该格子执行任何操作），同样是 $3$ 种方案，共 $27$ 种方案。第二个机器人的 $0$ 号格子要么输入输出都是空，要么输入和目标输出不同，是 $3$ 种方案，$1$ 号和 $2$ 号格子也都是 $3$ 种方案，共 $27$ 种方案。所以总共 $27 \times 27 = 729$ 种方案。</li>
<li>初始位置 $p = 1$ 可以使得执行完所有操作后满足条件。那么第一个机器人的纸带三个格子都是 $3$ 种方案，其中 $0$ 号格子要么输入输出都为空，要么相同；$1$ 号格子要么输入输出都为空，要么目标输出是 $1$；$2$ 号格子的输入输出要么都为空，要么输出是 $0$，共 $27$ 种方案。第二个机器人的 $1$ 号格子要么输入输出都是空，要么输入和目标输出不同，是 $3$ 种方案；$0$ 号和 $2$ 号格子要么输入输出都为空，要么输入输出相同，也都是 $3$ 种方案，共 $27$ 种方案。总共 $27 \times 27 = 729$ 种方案。</li>
<li>初始位置 $p = 2$ 可以使得执行完所有操作后满足条件。那么第一个机器人的纸带必须输入输出全为空（否则爆炸），只有 $1$ 种方案。第二个机器人是 $27$ 种方案，总共 $27$ 种方案。</li>
<li>初始位置 $p = 0, 1$ 都满足条件。这要求第一个机器人的 $1$ 号格子输入输出都为空；$0$ 号格子的输入输出都为空或都为 $1$；$2$ 号格子的输入输出都为空或都为 $0$，所以第一个机器人的纸带有 $4$ 种方案。第二个机器人 $0$ 号格子和 $1$ 号格子都为空，$2$ 号格子有 $3$ 种方案，第二个机器人的 $0$ 号和 $1$ 号格子必须都为空，$2$ 号格子要么输入输出都为空，要么输入和输出相同，有 $3$ 种方案。总共 $12$ 种方案。</li>
<li>初始位置 $p = 0, 2$ 都满足条件。那么第一个机器人的纸带必须输入输出全为空（否则爆炸），只有 $1$ 种方案。第二个机器人 $0$ 号和 $2$ 号格子都为空，$1$ 号格子有 $3$ 种方案。总共 $3$ 种方案。</li>
<li>初始位置 $p = 1, 2$ 都满足条件。那么第一个机器人的纸带必须输入输出全为空，只有 $1$ 种方案。第二个机器人 $1$ 号和 $2$ 号格子都为空，$0$ 号格子有 $3$ 种方案。总共 $3$ 种方案。</li>
<li>初始位置 $p = 0, 1, 2$ 都满足条件。那么两个机器人的输入输出必须都为空，总共 $1$ 种方案。</li>
</ol>
<p>根据容斥原理，最后的答案为 $729 + 729 + 27 - 12 - 3 - 3 + 1 = 1468$。</p>
<h2>样例三、样例四</h2>
<p>见样例数据下载。</p>
<h2>数据范围</h2>
<p>对于所有测试点：$1 \le n \le 32$，$1 \le m \le 1000$，$1 \le \lvert S_i \rvert \le 100$。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \le$</th>
<th style="text-align:center;">$m \le$</th>
<th style="text-align:center;">特殊限制</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 2$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$5 \sim 6$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$8 \sim 10$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$11 \sim 12$</td>
<td style="text-align:center;">$16$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">无</td>
</tr>
<tr>
<td style="text-align:center;">$13 \sim 15$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">A</td>
</tr>
<tr>
<td style="text-align:center;">$16 \sim 21$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">B</td>
</tr>
<tr>
<td style="text-align:center;">$22 \sim 25$</td>
<td style="text-align:center;">$32$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">无</td>
</tr>
</tbody>
</table>
</div>
<p>特殊限制 A：操作序列中不存在 <code>R</code>。</p>
<p>特殊限制 B：每个操作序列中，<code>R</code> 的数量至多 $15$ 个。 </p>
<p><strong>时间限制：$\texttt{3s}$</strong></p>
<p><strong>空间限制：$\texttt{1GB}$</strong></p>
