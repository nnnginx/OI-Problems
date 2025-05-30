<p><strong> 由于某些原因本题仅支持 C++, C++11 语言的提交。 </strong></p>
<p>滨海湾花园是新加坡的一个大型自然公园。公园内有 $n$ 个塔，称之为「擎天树」。这些塔的编号为 $0$ 到 $n-1$。我们希望建立一个桥的集合（桥的数目大于等于 $0$）。每一座桥连接两个不同的塔，而且可以双向通行。没有两座桥连接相同的一对塔。</p>
<p>一条从塔 $x$ 到塔 $y$ 的路径是一个满足以下条件的塔序列（塔的数目大于等于 $1$）：</p>
<ul>
<li><p>序列的第一个元素是 $x$，</p>
</li>
<li><p>序列的最后一个元素是 $y$，</p>
</li>
<li><p>序列中所有元素<strong>互不相同</strong>，</p>
</li>
<li><p>序列中每两个相邻元素（塔）都是被某一座桥连接起来的。</p>
</li>
</ul>
<p>注意根据定义，一个塔到它自己有且仅有一条路径，并且从塔 $i$ 到塔 $j$ 的不同路径的数目和从塔 $j$ 到塔 $i$ 的不同路径的数目是一样的。</p>
<p>负责该项设计的首席设计师希望待建造的桥梁要符合：任意给定 $0\le i,j\le n-1$，恰好有 $p_{i,j}$ 条从塔 $i$ 到塔 $j$ 的不同路径，其中 $0\le p_{i,j}\le 3$。</p>
<p>请构造一个桥的集合来满足设计师的要求，或判定这样的桥梁集合不可能存在。</p>
<h2>实现细节</h2>
<p>你必须引用 <code>supertrees.h</code> 头文件。</p>
<p>你需要实现下面的这个函数：</p>
<pre><code class="sh_cpp">int construct(std::vector&lt;std::vector&lt;int&gt;&gt; p)</code></pre>
<ul>
<li><p>$p$：一个表示设计师要求的 $n\times n$ 数组。</p>
</li>
<li><p>如果这个建设方案是存在的，该函数应该恰好调用一次 <code>build</code>（见下文）来给出建设方案，然后应返回 $1$。</p>
</li>
</ul>
<p>否则，该函数应该返回 $0$，并且不要调用 <code>build</code>。</p>
<p>该函数将被调用恰好一次。</p>
<p>函数 <code>build</code> 定义如下：</p>
<pre><code class="sh_cpp">void build(std::vector&lt;std::vector&lt;int&gt;&gt; b)</code></pre>
<ul>
<li>$b$：一个 $n\times n$ 的数组，$b_{i,j}=1$ 表示有一座桥连接塔 $i$ 和塔 $j$，否则 $b_{i,j}=0$。</li>
</ul>
<p>注意该数组必须满足：对所有 $0\le i,j\le n-1$，$b_{i,j} = b_{j,i}$；并且对所有 $0\le i\le n-1$，$b_{i,i}=0$。</p>
<h2>输入格式</h2>
<p>评测程序示例以如下格式读取输入数据：</p>
<ul>
<li>第 $1$ 行：$n$</li>
<li>第 $2+i$ 行（$0\le i\le n-1$）：$p_{i,0}\ p_{i,1}\ \cdots\ p_{i,n-1}$</li>
</ul>
<h2>输出格式</h2>
<p>评测程序示例的输出格式如下：</p>
<ul>
<li>第 $1$ 行: <code>construct</code> 的返回值。</li>
</ul>
<p>如果 <code>construct</code> 的返回值为 $1$，评测程序示例会额外打印：</p>
<ul>
<li>第 $2+i$ 行（$0\le i\le n-1$）：$b_{i,0}\ b_{i,1}\ \cdots\ b_{i,n-1}$</li>
</ul>


<pre><code class="language-input1">4
1 1 2 2
1 1 2 2
2 2 1 2
2 2 2 1
</code></pre>


<pre><code class="language-output1">1
0 1 1 1
1 0 0 0
1 0 0 1
1 0 1 0
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">construct([[1, 1, 2, 2], [1, 1, 2, 2], [2, 2, 1, 2], [2, 2, 2, 1]])</code></pre>
<p>这表明从塔 $0$ 到塔 $1$ 恰好有一条路径。对于所有其他的塔对 $(x, y) (0\le x &lt; y\le 3)$, 恰好有两条不同的路径连接塔 $x$ 和塔 $y$。这可以通过建设 $4$ 座桥来实现：连接塔对 $(0, 1), (1, 2), (1, 3)$ 和 $(2, 3)$。</p>
<p>为了给出这个解决方案，函数 <code>construct</code> 应该做以下调用：</p>
<ul>
<li><code>build([[0, 1, 0, 0], [1, 0, 1, 1], [0, 1, 0, 1], [0, 1, 1, 0]])</code></li>
</ul>
<p><img src="https://img.uoj.ac/problem/565/565_ex1.png" alt="样例一" class="img-responsive center-block" style="width:200px;"></p>
<p>函数应该返回 $1$。</p>
<p>对于这个例子，存在多种不同的建设方案来满足要求，所有这些方案都被认为是正确的。</p>


<pre><code class="language-input2">2
1 0
0 1
</code></pre>


<pre><code class="language-output2">1
0 0
0 0
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">construct([[1, 0], [0, 1]])</code></pre>
<p>这表明无法在两个塔之间进行旅行。这只能通过不建设桥梁来满足。</p>
<p>因此，函数 <code>construct</code> 应该做以下调用：</p>
<ul>
<li><code>build([[0, 0], [0, 0]])</code></li>
</ul>
<p>然后，函数 <code>construct</code> 应该返回 $1$。</p>


<pre><code class="language-input3">2
1 3
3 1
</code></pre>


<pre><code class="language-output3">0
</code></pre>


<p>考虑以下调用：</p>
<pre><code class="sh_cpp">construct([[1, 3], [3, 1]])</code></pre>
<p>这表明从塔 $0$ 到塔 $1$ 恰好有 $3$ 条路径。这些要求无法满足。因此，函数 <code>construct</code> 应该返回 $0$ 并且不要调用 <code>build</code>。</p>
<h2>限制与约定</h2>
<p>对于 $100\%$ 的数据，满足：</p>
<ul>
<li>$1\le n\le 1000$</li>
<li>$p_{i,i}=1$（对所有 $0\le i\le n-1$）</li>
<li>$p_{i,j}=p_{j,i}$（对所有 $0\le i,j\le n-1$）</li>
<li>$0\le p_{i,j}\le 3$（对所有 $0\le i, j\le n-1$）</li>
</ul>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">子任务</th>
<th style="text-align:center;">附加限制</th>
<th style="text-align:center;">分值</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$p_{i,j}=1$（对所有 $0\le i,j\le n-1$）</td>
<td style="text-align:center;">$11$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$p_{i,j}\in \{0,1\}$（对所有 $0\le i,j\le n-1$）</td>
<td style="text-align:center;">$10$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$p_{i,j}\in \{0,2\}$（对所有 $i\neq j,0\le i,j\le n-1$）</td>
<td style="text-align:center;">$19$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$0\le p_{i,j}\le 2$（对所有 $0\le i,j\le n-1$）并且至少有一种建设方案满足要求</td>
<td style="text-align:center;">$35$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$0\le p_{i,j}\le 2$（对所有 $0\le i,j\le n-1$）</td>
<td style="text-align:center;">$21$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">没有额外约束条件</td>
<td style="text-align:center;">$4$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1 \texttt{s}$</p>
<p><strong>空间限制</strong>：$1024 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20969/file/attachment.zip">样例及测评库下载</a></p>
