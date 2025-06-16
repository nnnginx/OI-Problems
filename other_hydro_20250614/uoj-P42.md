<p>给定正整数 $n, r$，求</p>
<div style="font-size:200%;">
\begin{equation}
\sum_{d = 1}^{n}{(-1)^{\left\lfloor \sqrt{d~\times~r~\times~d} \right\rfloor}}
\end{equation}
</div>

<h2>输入格式</h2>
<p>第一行一个数 $T$，表示有 $T$ 组测试数据。</p>
<p>接下来 $T$ 行，每行两个正整数 $n, r$。</p>
<h2>输出格式</h2>
<p>输出 $T$ 行，每行一个整数表示答案。</p>


<pre><code class="language-input1">3
3 5
3 6
3 7
</code></pre>


<pre><code class="language-output1">3
1
-1
</code></pre>

<h2>限制与约定</h2>
<p>对于 30% 的数据，满足 $n \leq 10^5, r \leq 10^2, T \leq 10$；</p>
<p>对于 60% 的数据，满足 $n \leq 10^7, r \leq 10^3, T \leq 10^2$；</p>
<p>对于 100% 的数据，满足 $n \leq 10^9, r \leq 10^4, T \leq 10^4$。</p>
<p><strong>时间限制</strong>：$1\texttt{s}$</p>
<p><strong>空间限制</strong>：$256\texttt{MB}$</p>
<h2>来源</h2>
<p>中国国家队清华集训2014~2015 Day 3 - By 罗雨屏</p>
<h2>下载</h2>
<p><a href="./20482/file/attachment.zip">样例数据下载</a></p>
