<p>已知多项式方程：</p>
<p>$$a_0+a_1x+a_2x^2+...+a_nx^n=0$$</p>
<p>求这个方程在$[1,m]$内的整数解（$n$和$m$均为正整数）。</p>
<h2>输入格式</h2>
<p>第一行包含$2$个整数$n$、$m$，每两个整数之间用一个空格隔开。</p>
<p>接下来的$n+1$行每行包含一个整数，依次为$a_0,a_1,a_2,...,a_n$。</p>
<h2>输出格式</h2>
<p>第一行输出方程在$[1,m]$内的整数解的个数。</p>
<p>接下来每行一个整数，按照从小到大的顺序依次输出方程在$[1,m]$内的一个整数解。</p>


<pre><code class="language-input1">2 10
1
-2
1
</code></pre>


<pre><code class="language-output1">1
1
</code></pre>



<pre><code class="language-input2">2 10
2
-3
1
</code></pre>


<pre><code class="language-output2">2
1
2
</code></pre>



<pre><code class="language-input3">2 10
1
3
2
</code></pre>


<pre><code class="language-output3">0
</code></pre>

<h2>限制与约定</h2>
<p>对于30%的数据，$0 &lt; n \le 2$，$|a_i| \le 100$，$a_n \ne 0$，$m \le 100$；</p>
<p>对于50%的数据，$0 &lt; n \le 100$，$|a_i| \le 10^{100}$，$a_n \ne 0$，$m \le 100$；</p>
<p>对于70%的数据，$0 &lt; n \le 100$，$|a_i| \le 10^{10000}$，$a_n \ne 0$，$m \le 10000$；</p>
<p>对于100%的数据，$0 &lt; n \le 100$，$|a_i| \le 10^{10000}$，$a_n \ne 0$，$m \le 1000000$。</p>
<p><strong>时间限制：</strong>$1\texttt{s}$</p>
<p><strong>内存限制：</strong>$128\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20460/file/attachment.zip">样例数据下载</a></p>
