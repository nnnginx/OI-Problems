<p>Arezou 和她的兄弟 Borzou 是双胞胎。他们收到的生日礼物是一套好玩的玩具火车。他们用它建了一个有 $n$ 个车站和 $m$ 段<strong>单向轨道</strong>的铁路系统。这些车站的编号是从 $0$ 到 $n-1$。每段轨道都始于某一车站，然后终于同一车站或其他车站。每个车站至少会有一段轨道以它为起点。</p>
<p>其中有些车站是<strong>充电车站</strong>。无论何时，如果火车抵达某个充电车站，它都会被充到满电。满电火车拥有足够的动力连续地驶过 $n$ 段轨道，但是如果不再充电的话，在即将进入第 $n+1$ 段轨道时它就会因电已用光而停车。</p>
<p>每个车站都有一个轨道开关，可以扳向任一以该车站为起点的轨道。火车从某个车站驶出时，驶向的正是该车站的开关所扳向的轨道。</p>
<p>这对双胞胎打算用他们的火车玩个游戏。他们已经分完了所有的车站：每个车站要么归 Arezou，要么归 Borzou。游戏里面只有一列火车。游戏开始时，这列火车停在车站 $s$，并且充满了电。为启动游戏，车站 $s$ 的拥有者把车站 $s$ 的开关扳向某个以 $s$ 为起点的轨道。随后他们启动火车，火车也就开始沿着轨道行驶。</p>
<p>无论何时，在火车首次进入某一车站时，该车站的拥有者都要扳定车站开关。开关一旦扳定，它就会保持状态不变直到游戏结束。因此，火车如果开到了某个曾经进过的车站，就会沿着与之前相同的轨道开出该车站。</p>
<p>由于车站数量是有限的，火车的行驶最终都会落入某个<strong>环路</strong>。环路是指一系列<strong>不同</strong>的车站 $c[0],c[1],\cdots,c[k-1]$，其中火车在离车站 $c[i]$（$\le i &lt; k-1$）后驶上连向车站 $c[i+1]$ 的轨道，在离开车站 $c[k-1]$ 后驶上连向车站 $c[0]$ 的轨道。一个环路可能只包括一个车站（此时 $k=1$），即火车从车站 $c[0]$ 驶出后又驶上了连向 $c[0]$ 的轨道。</p>
<p>如果火车能够连续行驶跑个没完，Arezou 就赢了。否则火车最后会把电用光而停车，这样 Borzou 就赢了。换句话说，如果在车站 $c[0],c[1],\cdots,c[k-1]$ 中至少有一个充电车站，且使得火车能够不断地充电而沿着环路跑个没完，Arezou 赢。否则，它就会最终把电用光（有可能是在沿着环路跑好几圈后），Borzou 赢。</p>
<p>现在给你一个这样的铁路系统。Arezou 和 Borzou 将会玩 $n$ 轮游戏。其中在第 $s$ 轮游戏中（$0\le s\le n-1$），火车最初停在车站 $s$ 上。你的任务是，对每一轮游戏，判断是否无论 Borzou 怎么玩，Arezou 都必胜。</p>
<h2>实现细节</h2>
<p><strong>本题只支持C++。</strong></p>
<p>你需要实现下面的函数：</p>
<pre><code class="sh_cpp"> std::vector&lt;int&gt; who_wins(std::vector&lt;int&gt; a, std::vector&lt;int&gt; r, std::vector&lt;int&gt; u, std::vector&lt;int&gt; v)</code></pre>
<ul>
<li>$a$：长度为 $n$ 的数组。如果 Arezou 拥有车站 $i$，则 $a[i]=1$；否则 Borzou 拥有车站 $i$，且 $a[i]=0$。</li>
<li>$r$：长度为 $n$ 的数组。如果车站 $i$ 是充电车站，则 $r[i]=1$。否则 $r[i]=0$。</li>
<li>$u$ 和 $v$：长度为 $m$ 的数组。对于所有 $0\le i\le m-1$，存在某一单向轨道，其起点为 $u[i]$，终点为 $v[i]$。</li>
<li>该函数需要返回一个长度为 $n$ 的数组 $w$。对于每个 $0\le i\le n-1$，如果在火车最初停在车站 $i$ 的游戏中，不管 Borzou 怎么玩，Arezou 都能赢，则 $w[i]$ 的值 1。否则 $w[i]$ 的值应为 $0$。</li>
</ul>
<h2>例子</h2>
<p>评测程序调用了 <code>who_wins([0, 1], [1, 0], [0, 0, 1, 1], [0, 1, 0, 1])</code>。</p>
<ul>
<li>这里有 $2$ 个车站。Borzou 拥有充电车站 $0$。Arezou 拥有车站 $1$，但是它不是充电车站。</li>
<li>这里有 $4$ 段轨道 $(0,0),(0,1),(1,0)$ 和 $(1,1)$，其中 $(i,j)$ 表示一个以车站 $i$ 为起点、车站 $j$ 为终点的单向轨道。</li>
<li>考虑火车最初停在车站 $0$ 的游戏。如果 Borzou 车站 $0$ 的开关扳向轨道 $(0,0)$，那么火车就会沿着这个环形轨道绕个没完（注意，车站 $0$ 是一个充电车站）。在这种情况下，Arezou 赢。否则，如果 Borzou 把车站 $0$ 的开关扳向轨道 $(0,1)$，Arezou 可以把车站 $1$ 的开关扳向轨道 $(1,0)$。这样的话，火车将会在两个车站之间绕个不停。Arezou 还是会赢，因为车站 $0$ 是充电车站，火车将跑个没完。因此，无论 Borzou 怎么玩，Arezou 都会赢。</li>
<li>根据类似的逻辑，在火车最初停在车站 $1$ 的游戏中，无论 Borzou 怎么玩，Arezou 也都会赢。因此，函数应当返回 $[1,1]$。</li>
</ul>
<h2>数据范围</h2>
<ul>
<li>$1\le n\le 5000$。</li>
<li>$n\le m\le 20\ 000$。</li>
<li>至少会有一个充电车站。</li>
<li>每个车站至少会有一段轨道以它为起点。</li>
<li>可能会有某个轨道的起点和终点是相同的（即 $u[i]=v[i]$）。</li>
<li>所有轨道两两不同。也就是说，不存在这样的两个下标 $i$ 和 $j$（$0\le i &lt; j\le m-1$），使得 $u[i]=u[j]$ 且 $v[i]=v[j]$。</li>
<li>对于所有 $0\le i\le m-1$，都有 $0\le u[i],v[i]\le n-1$。</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务编号</th>
<th style="text-align:center;">限制与约定</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">对于所有 $0\le i\le m-1$，都有 $v[i]=u[i]$ 或者 $v[i]=u[i]+1$</td>
<td style="text-align:center;">$5$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$n\le 15$</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">Arezou 拥有所有车站</td>
<td style="text-align:center;">$11$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">Borzou 拥有所有车站</td>
<td style="text-align:center;">$11$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">充电车站的数量为 $1$</td>
<td style="text-align:center;">$12$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">无附加限制</td>
<td style="text-align:center;">$51$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$2\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>评分程序样例</h2>
<p>评分程序样例会按照下述格式来读取输入数据：</p>
<ul>
<li>第 $1$ 行：$n\ m$</li>
<li>第 $2$ 行：$a[0]\ a[1]\ \cdots\ a[n-1]$</li>
<li>第 $3$ 行：$r[0]\ r[1]\ \cdots\ r[n-1]$</li>
<li>第 $4+i$ 行（对于所有 $0\le i\le m-1$）：$u[i]\ v[i]$</li>
</ul>
<p>评分程序样例会按照下述格式打印出 <code>who_wins</code> 的返回结果：</p>
<ul>
<li>第 $1$ 行：$w[0]\ w[1]\ \cdots\ w[n-1]$</li>
</ul>
<h2>下载</h2>
<p><a href="./20749/file/attachment.zip">样例数据与样例评测库下载</a></p>
