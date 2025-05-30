<p>W 王国中有 $n$ 个城市，快递公司会在任意两个不同的城市之间配送快递。作为快递公司的总管理员，你打算把公司分成若干个部门并让这些部门之间相互竞争，以此来提高配送快递的效率。</p>
<p>划分部门并不是一件容易事，它需要考虑很多因素。对于两个不同的城市 $i,j$，如果 $i \to j$ 和 $j \to i$ 是由两个不同的部门负责的，那么一个部门配送完快递后返程就会没有事做，这样会浪费时间。对于三个不同的城市 $i,j,k$，如果 $i,j,k$ 之间六种配送方式都是由同一个部门负责的，那么你会觉着这个部门垄断了这三个城市之间的快递运输，这样对整个公司是不利的。因此，你规定：</p>
<ul><li>对于两个不同的城市 $i,j$，$i \to j$ 和 $j \to i$ 必须由同一个部门负责。</li>
<li>对于三个不同的城市 $i,j,k$，它们之间六种配送关系不能由同一个部门负责。</li>
</ul><p>由于划分出的部门数目太多会不利于公司的管理，所以你需要求出划分出的最少部门数目 $m$。</p>
<h2>输入格式</h2>
<p>一行一个整数 $n$。</p>
<h2>输出格式</h2>
<p>你需要用方案来证明你的答案，所以本题你需要输出方案。</p>
<p>你需要输出 $n$ 行，每行 $n$ 个整数，第 $i$ 行第 $j$ 列的整数 $A_{i,j}$ 表示第 $i$ 个城市和第 $j$ 个城市之间的快递运输由第 $A_{i,j}$ 个部门负责。</p>
<p>形式化地，假设你求出的最少划分数目为 $m$，那么你输出的矩阵 $A$ 需要满足以下性质：</p>
<ul><li>对于 $\forall i,j$ 且 $i\neq j$， 都有 $1\le A_{i,j} \le m$ 并且 $A_{i,j}$ 为整数。</li>
<li>对于 $\forall i,j$， 都有 $A_{i,j}=A_{j,i}$。</li>
<li>对于 $\forall i$， 都有 $A_{i,i}=0$。</li>
<li>对于 $\forall i,j,k,i &lt; j &lt; k$，都有 $A_{i,j} \ ,A_{i,k} \ ,A_{j,k}$ 不完全相同。</li>
</ul><p><strong>你并不需要输出 $m$，在判断答案时会自动将你输出的数中的最大值作为 $m$。</strong></p>


<pre><code class="language-input1">3
</code></pre>


<pre><code class="language-output1">0 1 2
1 0 1
2 1 0
</code></pre>

<h2>限制与约定</h2>
<p><strong>本题是一道传统题，但表格中的限制为 $n=$ 并非 $n\le$。</strong></p>
<p>如果你输出的方案不合法，那么该测试点得 $0$ 分。</p>
<p>如果你输出的方案所对应 $m$ 不是最少的划分数，那么该测试点得 $0$ 分。</p>
<p>否则，每个测试点的信息如下：</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>1</th>
<th>2</th>
<th>3</th>
<th>4</th>
<th>5</th>
<th>6</th>
<th>7</th>
<th>8</th>
<th>9</th>
<th>10</th>
</tr></thead><tbody><tr><td>$n=$</td>
<td>5</td>
<td>8</td>
<td>16</td>
<td>25</td>
<td>32</td>
<td>33</td>
<td>34</td>
<td>80</td>
<td>82</td>
<td>85</td>
</tr><tr><td>分值</td>
<td>5</td>
<td>5</td>
<td>10</td>
<td>10</td>
<td>5</td>
<td>10</td>
<td>20</td>
<td>5</td>
<td>10</td>
<td>20</td>
</tr></tbody></table></div>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./21003/file/attachment.zip">样例数据下载</a></p>
