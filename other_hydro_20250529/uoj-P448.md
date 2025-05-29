<p>小A和小C在玩一个游戏，每次小A从$1$~$n$中任意选择一个数$i$，然后小C从$1$~$i$中任意选择一个数$x$，这将会产生$\gcd(i,x)$的价值。众所周知，小C是一个复读机，他会重复$k$次这样的操作，游戏的总价值为每次小C产生价值的最小公倍数。</p>
<p>现在小A想要知道所有情况下游戏总价值的和是多少，由于一些显而易见的原因，你只需要求出在模$10^9+7$意义下的和即可。</p>
<h2>输入格式</h2>
<p>一行两个正整数$n,k$。</p>
<h2>输出格式</h2>
<p>一行一个整数，表示游戏的价值和。</p>


<pre><code class="language-input1"><code>3 1</code>
</code></pre>

<pre><code class="language-output1"><code>9</code>
</code></pre>

<p>对于Sample Input 1 价值为
$\gcd(1,1)+\gcd(2,1)+\gcd(2,2)+\gcd(3,1)+\gcd(3,2)+\gcd(3,3)=9$</p>


<pre><code class="language-input2"><code>5 2</code>
</code></pre>

<pre><code class="language-output2"><code>130</code>
</code></pre>


<pre><code class="language-input3"><code>1000000 1000</code>
</code></pre>

<pre><code class="language-output3"><code>763267594</code>
</code></pre>
<h2>限制与约定</h2>
<p>$1 \le n \le 10^9, 1 \le k \le 10^9, 1 \le n*k \le 10^9$</p>
<p>本题使用子任务评测（空则表示无特殊性质）</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-verticle-middle"><thead><tr><th>子任务</th><th>分值</th><th>$n$</th><th>$k$</th></tr></thead><tbody><tr><td>1</td><td>5</td><td>$\leq 10^6$</td><td>$= 1$</td></tr><tr><td>2</td><td>5</td><td>&nbsp;</td><td>$= 1$</td></tr><tr><td>3</td><td>7</td><td>$\leq 10^6$</td><td>$= 2$</td></tr><tr><td>4</td><td>8</td><td>&nbsp;</td><td>$= 2$</td></tr><tr><td>5</td><td>35</td><td>$\leq 10^7$</td><td>&nbsp;</td></tr><tr><td>6</td><td>40</td><td>&nbsp;</td><td>&nbsp;</td></tr></tbody></table></div>


<p><strong>时间限制：$\texttt{2s}$</strong></p>
<p><strong>空间限制：$\texttt{512MB}$</strong></p>
<h2>下载</h2>
<p><a href="./20853/file/attachment.zip">样例数据下载</a></p>
