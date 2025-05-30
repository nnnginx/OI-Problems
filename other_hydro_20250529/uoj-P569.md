<p><strong> 如果本题评测出现问题，请联系管理员。 </strong></p>
<p>新加坡的互联网主干网由 $n$ 个网络站点组成，这些站点分配了从 $0$ 到 $n-1$ 的序号。互联网中还有 $n-1$ 条双向链路，它们从 $0$ 到 $n-2$ 编号。每条链路连接两个不同的站点。被一条链路连接着的两个站点互相称作对方的邻居。</p>
<p>一个由互不相同的站点所组成的站点序列 $a_0, a_1, \cdots, a_p$ 被称作一条从站点 $x$ 到站点 $y$ 的路径，当且仅当 $a_0 = x$，$a_p = y$，并且序列中每两个连续的站点都是邻居。保证从任意站点 $x$ 到任意其他站点 $y$ 有且仅有一条路径。</p>
<p>任意站点 $x$ 可以生成一个数据包，并把它发送给任意其他站点 $y$，站点 $y$ 称作这个数据包的<strong>目的站点</strong>。数据包需要按下述规则在站点 $x$ 到站点 $y$ 的唯一路径上进行路由。假设数据包当前发送到了站点 $z$，其中 $y$ 是数据包的目的站点且 $z \ne y$，则站点 $z$ 会：</p>
<ol>
<li>执行<strong>路由函数</strong>，找到 $z$ 到 $y$ 的唯一路径中 $z$ 的邻居。然后</li>
<li>将数据包转发给这个邻居。</li>
</ol>
<p>然而，站点有存储内存限制，可能无法存下路由函数中需要使用的完整的主干网链路列表。</p>
<p>你的任务是实现主干网的路由机制，它由两个函数组成：</p>
<ul>
<li>第一个函数的输入参数为 $n$、主干网链路的列表和一个整数 $k \ge n - 1$。该函数需要为每个站点分配一个独一无二的<strong>编号</strong>，其大小在 $0$ 到 $k$ 之间（包括 $0$ 和 $k$）。</li>
<li>第二个函数是路由函数，它在站点编号分配好后部署到所有站点上。<ul>
<li>它的输入参数如下：<ul>
<li>$s$，数据包当前所处的站点的<strong>编号</strong>，</li>
<li>$t$，数据包的目的站点的<strong>编号</strong>（$t \ne s$），</li>
<li>$c$，表示 $s$ 的所有邻居站点的<strong>编号</strong>的列表。</li>
</ul>
</li>
<li>该函数应该返回一个 $s$ 的邻居的<strong>编号</strong>，表示数据包需要转发到的下个站点。</li>
</ul>
</li>
</ul>
<p>在每个子任务中，你的得分取决于所有站点被分配到的编号的最大值（通常来说，编号最大值越小越好）。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>stations.h</code> 头文件。</p>
<p>你需要实现下列函数：</p>
<pre><code class="sh_cpp">int[] label(int n, int k, int[] u, int[] v)</code></pre>
<ul>
<li>$n$：主干网中站点的数量。</li>
<li>$k$：可用的编号的最大值。</li>
<li>$u$ 和 $v$：大小为 $n - 1$ 的数组，表示链路。对每个 $i$（$0 \le i \le n - 2$），链路 $i$ 连接着序号为 $u[i]$ 和 $v[i]$ 的站点。</li>
<li>该函数应该返回一个大小为 $n$ 的数组 $L$。对每个 $i$（$0 \le i \le n-1$），$L[i]$ 表示序号为 $i$ 的站点所分配到的编号。数组 $L$ 中的所有元素必须互不相同并且大小在 $0$ 到 $k$ 之间。</li>
</ul>
<pre><code class="sh_cpp">int find_next_station(int s, int t, int[] c)</code></pre>
<ul>
<li>$s$：数据包当前所在站点的编号。 </li>
<li>$t$：数据包目的站点的编号。 </li>
<li>$c$：一个数组，包含 $s$ 的所有邻居的编号。数组 $c$ 按照元素大小升序排列。 </li>
<li>该函数应该返回一个 $s$ 的邻居的编号，表示数据包需要转发到的下个站点。</li>
</ul>
<p>每个测试用例包含一个或多个独立的场景（也就是不同的主干网描述）。对于一个包含 $r$ 个场景的测试用例，调用上述函数的评测程序会按下列步骤运行恰好两次。 </p>
<p>程序第一次运行期间： </p>
<ul>
<li><p><code>label</code> 函数被调用 $r$ 次，</p>
</li>
<li><p>返回的编号将被评测系统保存，并且</p>
</li>
<li><p><code>find_next_station</code> 不会被调用。 </p>
</li>
</ul>
<p>程序第二次运行期间： </p>
<ul>
<li><p><code>find_next_station</code> 会被调用若干次。对于每次调用，评测程序会选择任意某个场景，该场景中的 <code>label</code> 函数所返回的编号方式将用于本次 <code>find_next_station</code> 调用。</p>
</li>
<li><p>label 不会被调用。</p>
</li>
</ul>
<p>特别地，在评测程序第一次运行期间，保存在静态或全局变量中的信息将无法在 <code>find_next_station</code> 函数中使用。 </p>
<h2>例子</h2>
<p>考虑下列调用：</p>
<pre><code class="sh_cpp">label(5, 10, [0, 1, 1, 2], [1, 2, 3, 4])</code></pre>
<p>共有 $5$ 个站点和 $4$ 条链路，链路对应的站点序号对分别为$ (0,1),(1,2),(1,3)$ 和 $(2,4)$。编号的大小范围为 $0$ 到 $k=10$。</p>
<p>为了返回下列编号方案：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>序号</th>
<th>编号</th>
</tr>
</thead>
<tbody>
<tr>
<td>0</td>
<td>6</td>
</tr>
<tr>
<td>1</td>
<td>2</td>
</tr>
<tr>
<td>2</td>
<td>9</td>
</tr>
<tr>
<td>3</td>
<td>3</td>
</tr>
<tr>
<td>4</td>
<td>7</td>
</tr>
</tbody>
</table>
</div>
<p>函数 <code>label</code> 应该返回 $[6, 2, 9, 3, 7]$。下图中的数字表示站点的序号（左图）与分配到的编号（右图）。 </p>
<p><img src="https://img.uoj.ac/problem/569/ex1.png" alt="" class="img-responsive center-block" style="width:400px;"></p>
<p>假设编号按照上图所示进行分配，考虑下列的调用：</p>
<pre><code class="sh_cpp">find_next_station(9, 6, [2, 7])</code></pre>
<p>它表示数据包当前所处的站点编号为 $9$，其目的站点的编号为 $6$。从当前站点到目的站点的路径上， </p>
<p>站点编号依次为 $[9,2,6]$。因此，函数应该返回 $2$，表示数据包应该转发给编号为 $2$ 的站点（其序号为 $1$）。 </p>
<p>考虑另一个可能的调用： </p>
<pre><code class="sh_cpp">find_next_station(2, 3, [3, 6, 9])</code></pre>
<p>该函数应该返回 $3$，因为目的站点（编号 $3$）是当前站点（编号 $2$）的邻居，因此目的站点直接接收到了数据包。</p>
<h2>约束条件</h2>
<ul>
<li>$1 \leq r \leq 10$</li>
</ul>
<p>对于 <code>label</code> 的每次调用：</p>
<ul>
<li>$2 \leq n \leq 1000$</li>
<li>$k \geq n-1$</li>
<li>$ 0 \leq u[i], v[i] \leq n-1$ （对于所有 $0 \leq i \leq n-2$）</li>
</ul>
<p>对于 <code>find_next_station</code> 的每次调用，其输入参数来自于任意选择的某次之前对 <code>label</code> 的调用。 </p>
<p>考虑它所产生的编号， </p>
<ul>
<li><p>$s$ 和 $t$ 是两个不同站点的编号。 </p>
</li>
<li><p>$c$ 是编号为 $s$ 的站点的所有邻居的编号的序列，升序排列。</p>
</li>
</ul>
<p>对于每个测试用例，所有场景加到一起，传递给函数 <code>find_next_station</code> 的所有数组 $c$ 的总长度不超过 $100000$。</p>
<h2>子任务</h2>
<ol>
<li>（5分）$k=1000$，不会出现拥有多于 $2$ 个邻居的站点。</li>
<li>（8分）$ k=1000$，链路 $i$ 连接站点 $i+1$ 和 $\left\lfloor\frac{i}{2}\right\rfloor$。</li>
<li>（16分）$k=1000000$，最多一个站点拥有多于 $2$ 个的邻居。</li>
<li>（10分）$n \leq 8, k=10^{9}$</li>
<li>（61分）$k=10^{9}$</li>
</ol>
<p>在子任务 5 中，你可以获得部分分。 令$m$为所有场景中 <code>label</code> 返回的最大编号。 对于这个子任务，你的得分将根据下表计算得到：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th>最大编号</th>
<th>得分</th>
</tr>
</thead>
<tbody>
<tr>
<td>$m \geq 10^9$</td>
<td>$0$</td>
</tr>
<tr>
<td>$2000\leq m \lt 10^9$</td>
<td>$50 \cdot \log _{5 \cdot 10^{5}}\left(\frac{10^{9}}{m}\right)$</td>
</tr>
<tr>
<td>$1000\lt m \lt 2000$</td>
<td>$50$</td>
</tr>
<tr>
<td>$m \leq 1000$</td>
<td>$61$</td>
</tr>
</tbody>
</table>
</div>
<h2>评测程序示例</h2>
<p>评测程序示例以如下格式读取输入数据：</p>
<ul>
<li>第$1$行：$r$</li>
</ul>
<p>接下来是 块内容，每块描述了一个单独的场景，格式如下： </p>
<ul>
<li>第$1$行：$n$ $k$</li>
<li>第 $2+i$（$0 \leq i \leq n-2$）行: $u[i] v[i]$</li>
<li>第 $1+n$ 行： $q$，<code>find_next_station</code> 的调用次数</li>
<li>第 $2+n+j$（$0 \leq j \leq q-1$）行: $z[j]$ $y[j]$ $w[j]$，第 $j$ 次调用 <code>find_next_station</code> 时所涉及的站点的<strong>序号</strong>。此时，数据包在站点 $z[j]$，目的站点为 $y[j]$，应该要转发给站点 $w[j]$。</li>
</ul>
<p>评测程序示例以如下格式打印你的结果：</p>
<ul>
<li>第$1$行：$m$</li>
</ul>
<p>接下来是 $r$ 块内容，分别对应输入中的场景。每块的格式如下：</p>
<ul>
<li>第$1+j$（$0 \leq j \leq q-1$）行：站点的<strong>序号</strong>，它所对应的<strong>编号</strong>是第 $j$ 次调用 <code>find_next_station</code> 时返回的结果。</li>
</ul>
<p>注意：评测程序示例每次执行时会同时调用 <code>label</code> 和 <code>find_next_station</code>。</p>
<h2>hack</h2>
<p>在 <code>hack</code> 时，数据格式与上述类似，但是您需要在最后额外添加一行两个数，第一个数为 <code>0/1</code>，表示是否给予部分分，第二个数为 $[0, 2^{31}-1]$ 内的整数，为打乱询问顺序的种子。</p>
<h2>限制与约定</h2>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$1\texttt{GB}$</p>
<h2>下载</h2>
<p><a href="./20973/file/attachment.zip">样例及测评库下载</a></p>
