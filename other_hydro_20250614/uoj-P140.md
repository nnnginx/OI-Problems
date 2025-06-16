<p>很久很久以前，有一个数字加入了 UOJ 群。</p>
<p>这天，在它讨论“一个数字应该怎么取模”的时候一不小心被删除了，变成了被粉碎的数字。</p>
<p>突然间，它突然发现它忘记了自己是谁。这让它感觉很焦躁，于是它来拜托你来帮它找到它所代表的整数 $x$。</p>
<p>在经过一番询问之后，你整理了一下现在你得到的线索：</p>
<ol><li>已知整数 $R$，有 $1 \leq x \leq R$</li>
<li>定义函数 $f(x)$ 为 $x$ 的各位数字之和，例如 $f(13)=4,f(233)=8$。已知整数 $k$，有 $f(x)=f(k \times x)$</li>
</ol><p>然而遗憾的是，你发现即使拥有了这些条件，可能的 $x$ 依然有很多个。因此，为了进一步缩小排查范围，你想要知道满足这两个条件的整数有多少个。</p>
<h2>输入格式</h2>
<p>仅一行两个正整数 $R$ 和 $k$。</p>
<h2>输出格式</h2>
<p>仅一个整数，表示可能的整数 $x$ 有多少个。</p>
<p>C/C++ 输入输出 long long 时请用 <code>%lld</code>。C++ 可以直接使用 cin/cout 输入输出。</p>


<pre><code class="language-input1">100 1
</code></pre>


<pre><code class="language-output1">100
</code></pre>


<p>因为对于所有的正整数 $x$ 都有 $f(x)=f(x)$，所以答案就是 $R$，即100。</p>


<pre><code class="language-input2">10 3
</code></pre>


<pre><code class="language-output2">1
</code></pre>


<p>只有⑨是满足条件的。</p>


<pre><code class="language-input3">666666666 233
</code></pre>


<pre><code class="language-output3">15272224
</code></pre>

<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>测试点编号</th>
<th>$R$的规模</th>
<th>$k$的规模</th>
</tr></thead><tbody><tr><td>1</td><td rowspan="2">$R \leq 10^6$</td><td rowspan="5">$k &lt; 1000$</td></tr><tr><td>2</td></tr><tr><td>3</td><td rowspan="3">$R \leq 10^8$</td></tr><tr><td>4</td></tr><tr><td>5</td></tr><tr><td>6</td><td rowspan="5">$R \leq 10^{18}$</td><td rowspan="2">$k &lt; 10$</td></tr><tr><td>7</td></tr><tr><td>8</td><td rowspan="3">$k &lt; 1000$</td></tr><tr><td>9</td></tr><tr><td>10</td></tr></tbody></table></div>

<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>空间限制：</strong>$256\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20580/file/attachment.zip">样例数据下载</a></p>
